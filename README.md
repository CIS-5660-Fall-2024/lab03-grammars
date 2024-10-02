# lab03-grammars
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## 1. Wheat grammar puzzle
Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output. Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

### Solution
![image](https://github.com/user-attachments/assets/c9ef6597-9be7-4f98-858e-58a86dc9cd01)
### Result
n = 1  
![image](https://github.com/user-attachments/assets/43239282-8cf4-485e-af7d-a2a72379a4fe)
n = 2  
![image](https://github.com/user-attachments/assets/55732a60-d67e-475f-88a9-d6142c66f738)
n = 3  
![image](https://github.com/user-attachments/assets/0bd4ca73-2441-4cbb-8171-33fb57df04ef)

## 2. Square grammar puzzle
How about this one? Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

### Solution
![image](https://github.com/user-attachments/assets/3b6d95b0-bd5b-41e0-a42e-f94c89a0046b)
![image](https://github.com/user-attachments/assets/4b23c6a2-e938-4025-9a86-618721e6df03)
### Result
n = 1  
![image](https://github.com/user-attachments/assets/e853d0f5-0ee0-4b45-ac74-924a72955795)
n = 2  
![image](https://github.com/user-attachments/assets/7d3a240c-5599-43b9-bdb3-71df6b6730fa)
n = 3  
![image](https://github.com/user-attachments/assets/5fa37395-d343-463a-92d1-a64c04a75e79)

## 3. Custom plant
Choose a plant in the world. Working off a reference, design a grammar that mimics the structure of that plant. Unlike our simple puzzles, please use multiple rules for greater complexity. Think carefully about the structure of your grammar! EXPLAIN the structure of your plant in the README. What are the components? What do each of the rules do? Be sure to also include images of a few iterations of your output plant.
### Result
![image](https://github.com/user-attachments/assets/a53d0e44-ae39-4f4d-adc3-f30636d17063)
### Rules
![image](https://github.com/user-attachments/assets/0bffcf5b-79c9-4586-b092-3c379c40f4e8)
![image](https://github.com/user-attachments/assets/7c62f030-eb63-452d-8522-4c9a004c47c4)
![image](https://github.com/user-attachments/assets/ec0dc7e2-820f-4d1e-a8ac-369b8a9e5fd6)
Here’s a short explanation based on your L-System and the plant structure in the image:

### Explanation of the Plant Structure

- **Premise (FX):** The starting point of the plant structure. `F` represents the forward growth, while `X` is a placeholder for recursive branching.
  
- **Rule 1 (X → F[+X][-X]F+X-):** 
    - `F[+X][-X]F+X-` is the core branching rule.
    - `F` extends the current branch.
    - `[+X]` and `[-X]` create two new branches diverging at different angles (`+` for clockwise and `-` for counterclockwise).
    - The last `+X-` ensures continued growth and further recursion for the branching process.

- **Rule 2 (F → FF):** This doubles the length of any segment `F`, allowing for longer stems and branches as the plant grows over iterations.

## Submission
- Create a pull request against this repository
- In your readme, list your solutions and format your README nicely
- Profit
