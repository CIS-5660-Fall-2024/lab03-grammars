# lab03-grammars
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.\
Team: Jill Rayca and Clara Nolan


## 1. Wheat grammar puzzle
Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output. Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">\
Rules:\
![rules1grammars](https://github.com/user-attachments/assets/8e63b1f0-a014-4697-b9d1-e8efc1ee2044)

## 2. Square grammar puzzle
How about this one? Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">\
Rules:\
![rules2grammars](https://github.com/user-attachments/assets/40fa388b-1916-4252-90cf-f25cfb67dd51)


## 3. Custom plant
We decided to create a creosote bush, which are native to the Mojave desert, and a good build off of the skills learned in 1 and 2.\
![creosote](https://github.com/user-attachments/assets/2c30e700-e822-4e05-9379-fc83bf21d075)
\
Rule 1: X → X=[+F[+X][-X]FX][-F[+X][-X]FX]FFX\

Purpose: Models the main symmetric branches of the bush, where I wanted each branch to have 2 little forks to simulate how wide the plant is.\

Rule 2: F → FF\

Purpose: Simulates the height of the main middle branch and other sub branches by just drawing straight up twice.\
![sol3](https://github.com/user-attachments/assets/12663105-3421-4885-9086-2274e7d901a8)
![creo1](https://github.com/user-attachments/assets/8c3bfca4-5e57-44c7-b2f2-0a6815cdc5bd)
![creo2](https://github.com/user-attachments/assets/28d07a57-3b15-4e7f-b664-97aa3187924e)

## Submission
- Create a pull request against this repository
- In your readme, list your solutions and format your README nicely
- Profit
