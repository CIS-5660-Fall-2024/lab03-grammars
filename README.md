# lab03-grammars
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## 1. Wheat grammar puzzle
Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output. Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

![image](https://github.com/user-attachments/assets/0c967c27-3d7b-4be7-b23b-33d9bf9e8570)  
Premise: F   
Rule: F = FF[-F]F[-F]F-  
Angle: 20  

## 2. Square grammar puzzle
How about this one? Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

![image](https://github.com/user-attachments/assets/d48fa15c-9fc0-48ac-bfac-c275e6ed3a02)  
Premise: X  
Rules: X = -F  
F = F-F+F+F-F  
Angle: 90  

## 3. Custom plant
Choose a plant in the world. Working off a reference, design a grammar that mimics the structure of that plant. Unlike our simple puzzles, please use multiple rules for greater complexity. Think carefully about the structure of your grammar! EXPLAIN the structure of your plant in the README. What are the components? What do each of the rules do? Be sure to also include images of a few iterations of your output plant. 
I picked a gumbo limbo tree:   
![image](https://github.com/user-attachments/assets/b3166182-c6ae-4085-a3f2-0fc8ad4bdb1c)  
Here is my result after 10 iterations:  
![image](https://github.com/user-attachments/assets/80eb5749-1660-4029-93e5-cb6fc110210d)  
Here is it after 8 iterations:  
![image](https://github.com/user-attachments/assets/469ea65a-c00b-45d2-b21a-123d4238a434)  
Here is it after 7 iterations:  
![image](https://github.com/user-attachments/assets/1ed236cb-a4bb-40cf-8a24-2f6a4b846fa0)  

I had a bended plane as an additional J component, meant to mimick a leaf.  
Premise: FFFA  
Rules:  
A = [B]///[B]///[B]////B  
B = F&FFCJ  
C = [B]/////F[A]///////F[B]  

A represents a split into four directions.   
B has the leaf, and is where most branches end, but has a hidden bud (C) to keep expanding.  
C splits into three, but the branches are offset, adding more variation.  

## Submission
- Create a pull request against this repository
- In your readme, list your solutions and format your README nicely
- Profit
