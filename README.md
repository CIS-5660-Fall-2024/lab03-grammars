# lab03-grammars
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## Solutions
by Andrew Ding

1. with an angle of 20 degrees,

![rules_1](images/p1rules.png)

2. with an angle of 90 degrees,

![rules_2](images/p2rules.png)

3.

I chose the dragon blood tree.

reference:

![ref_3](images/p3ref.png)

rules for generation:

![rules_3](images/p3rules.png)

generated attempt (shown at 10 generations)

![gen_3](images/p3result.png)

There are visually two distinct parts to the tree; the branches which multiply quickly and the leaves which are short and thin.

The leaves exhibit no fractal pattern, which made it very difficult to find rules that had no generation limit. Duplication with a L-system is mainly accomplished by duplicating a symbol (e.g. A <- AA) and allowing that symbol to generate fully. There is a symbol for the leaves, L, but that symbol can't be duplicated because the leaves should only be drawn once; consequently, the generation where L is replaced by draw commands is the last one. (It's probably possible to find a different solution with other L-system capabilities, but I think it would be arduous.) 

In this case, after the 7th generation the L-system is stationary. I used a symbol variable for B to keep track of the number of generations; B is also used to generate the branches, which were allowed to proliferate until the 6th generation. Random rotations of the branches ended up frequently looking bad; the tree was pretty much always asymmetric, so I just used four deterministically-rotated branches in each generation.

The results aren't perfect. A lot depends on the length/thickness scale per branch (in the B(i) rule), as well as the branch pitch (currently 30 degrees) each generation. I think that for a more accurate tree, the branch pitch can't be the same across all generations.

Because of the finite-generation approach, in the intermediate generations the tree is bare of leaves:

![midgen_3](images/p3midgen.png)


## 1. Wheat grammar puzzle
Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output. Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

## 2. Square grammar puzzle
How about this one? Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

## 3. Custom plant
Choose a plant in the world. Working off a reference, design a grammar that mimics the structure of that plant. Unlike our simple puzzles, please use multiple rules for greater complexity. Think carefully about the structure of your grammar! EXPLAIN the structure of your plant in the README. What are the components? What do each of the rules do? Be sure to also include images of a few iterations of your output plant. 

## Submission
- Create a pull request against this repository
- In your readme, list your solutions and format your README nicely
- Profit
