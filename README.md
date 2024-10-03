# lab03-grammars
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## 1. Wheat grammar puzzle
Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output. Take a screenshot of your rules.\
<img width="565" alt="Screenshot 2024-10-02 at 9 16 46 PM" src="https://github.com/user-attachments/assets/461d9a24-574b-49da-beb0-65c405082d9c">\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

## 2. Square grammar puzzle
How about this one? Take a screenshot of your rules.\
<img width="577" alt="Screenshot 2024-10-02 at 9 18 31 PM" src="https://github.com/user-attachments/assets/f9683dde-0658-4fa8-bf6a-63f177cb6206">\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

## 3. Custom plant
Choose a plant in the world. Working off a reference, design a grammar that mimics the structure of that plant. Unlike our simple puzzles, please use multiple rules for greater complexity. Think carefully about the structure of your grammar! EXPLAIN the structure of your plant in the README. What are the components? What do each of the rules do? Be sure to also include images of a few iterations of your output plant.\
## Baby's Breath Reference:
<img width="350" src="https://github.com/user-attachments/assets/588fe0e2-d1a3-48c7-9f93-4390e705d158">\
I chose the flower baby's breath as my reference. The plants components can primarily be broken down into the main stem, left branches, right branches, and middle branches. And the symmetrical branching from each stem gets smaller and smaller.

<img width="300" alt="Screenshot 2024-10-02 at 10 09 20 PM" src="https://github.com/user-attachments/assets/d1bd5171-4054-42ae-9a47-8aaf0b4aa464">
<img width="300" alt="Screenshot 2024-10-02 at 10 09 39 PM" src="https://github.com/user-attachments/assets/04ab938e-13d4-4173-b4bb-3bdcc19dcd72">
<img width="300" alt="Screenshot 2024-10-02 at 10 09 54 PM" src="https://github.com/user-attachments/assets/713c9a14-1995-4a0e-aff2-28a7e72b9885">\


<img width="537" alt="Screenshot 2024-10-02 at 10 08 56 PM" src="https://github.com/user-attachments/assets/beddaba3-0c09-40ca-8d59-84aabd4d4ec4">\

Rules:\
X=[-FX]F[+FX][FX]
- [-FX] creates a right branch by turning right, going forward, then recursively repeating
- F offsets the flower to the right by going forward
- [+FX] creates a left branch by turning left, going forward, then recursively repeating
- [FX] creates the middle branch straight from the main stem, and recursively repeating

F=FF
- FF lengthens the stem each step every iteration, making it look like its growing

## Submission
- Create a pull request against this repository
- In your readme, list your solutions and format your README nicely
- Profit
