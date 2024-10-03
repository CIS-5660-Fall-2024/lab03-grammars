# lab03-grammars
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## 1. Wheat grammar puzzle
Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output. Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">
- Axiom: F
- Rule: F=FFF[+FF]F[+FF]FF+
- 20 deg
- <img width="499" alt="image" src="https://github.com/user-attachments/assets/3c3fe231-bc94-47c0-bb03-01182adb17b2">

## 2. Square grammar puzzle
How about this one? Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

- Axiom: +F
- Rule; F=F+F-F-F+F
- 90 deg
- <img width="715" alt="image" src="https://github.com/user-attachments/assets/585a0bdc-3548-4414-a733-b605fd6c2053">

## 3. Custom plant
tomato plant (sort of, I slightly dont know what i did)

<img width="691" alt="image" src="https://github.com/user-attachments/assets/5b74bbe8-e639-4609-87c7-dd5a7b3afd0b">
<img width="407" alt="image" src="https://github.com/user-attachments/assets/d0bc8b91-e1df-492d-963d-b91ea8282e7a">

Most of my rules are just me messing around in Houdini until something worked
- The premise is simply a stem going forward, then four leaves rotated around by 90, and then continued by X
- The A rule builds a leaf, angling a forward vine up and then placing the leaf
- X: To make the branches for each tomato vine, we move forward, go off on a tiny branch to make a leaf, go back then move forward, save three times to build each tomato vine, and then move forward
- B: To build the tomato, we make two tomatoes branch off, go forward, and then repeat but slightly tipped over

Special thanks to Lewis Ghrist for helping me make the leaves.

Reference:
![image](https://github.com/user-attachments/assets/1df09853-0b08-464a-8df1-3baa865fc092)
