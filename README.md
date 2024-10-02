# lab03-grammars (Charles Wang)
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## 1. Wheat grammar puzzle
Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output. Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

### Grammar

- Angle of `20`
- Premise: `F`
- Rule 1: `F=FF[+FF]F[+FF]FF+`

![image](https://github.com/user-attachments/assets/c6cc297f-4be7-4692-981a-5dbda674763f)

## 2. Square grammar puzzle
How about this one? Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

### Grammar

- Angle of `90`
- Premise: `F`
- Rule 1: `F=FF[+FF]F[+FF]FF+`

![image](https://github.com/user-attachments/assets/c9a442ce-cffa-4a1b-86fa-6cf7f4f345c1)

## 3. Custom plant
Choose a plant in the world. Working off a reference, design a grammar that mimics the structure of that plant. Unlike our simple puzzles, please use multiple rules for greater complexity. Think carefully about the structure of your grammar! EXPLAIN the structure of your plant in the README. What are the components? What do each of the rules do? Be sure to also include images of a few iterations of your output plant. 

### Acacia tree grammar

For my custom plant I tried recreating the look of an acacia plant from this reference image:

![image](https://github.com/user-attachments/assets/77e16ef4-ed79-45d7-93cb-d971cf5d24d0)

I ended up with this grammar:

- Angle of `15`
- Rule 1: `A=""[B]////////"[C]`
- Rule 2: `B=&FFF[^^^^FF]FFFA`
- Rule 3: `C=&&&FFFBA """" B`

A couple of generations (click the image to see full resolution, they're kinda small in the README):

| 7 generations | 10 generations | 14 generations |
|---------------|----------------|----------------|
|![image](https://github.com/user-attachments/assets/7d2c14ce-74a3-4f0f-a520-6c10b99b6fc2)|![image](https://github.com/user-attachments/assets/4ee3fcf4-a2c2-461c-bc2b-f22fa1829522)|![image](https://github.com/user-attachments/assets/73e3dd63-7999-45ee-bcf3-c93adfa972f7)|

I think generations 10 or 14 look the best and match the reference the best. To explain my rules: I chose a smaller angle because each iteration should have small rotations but as you travel up the branches, they should progressively add on to each other. Rule 1 holds the basic structure of the tree, creating two branches at each "level" that are facing away from each other. This rule also reduces the lengths of each branch drastically, matching the smaller branches seen in the top levels of the acacia tree.

Rules 2 and 3 take care of the "left" and "right" branches respectively from rule 1. In particular, rule 3 includes both rule 2 and two references of rule 3 because there are a lot of branches in the upper-right area of the reference image. Rule 2 has less branches and they're far longer, so it only includes one reference to rule 1 to keep the recursion going.
