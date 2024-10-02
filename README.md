# lab03-grammars
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## 1. Wheat grammar puzzle
Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output. Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

```
Angle: 20
Axiom: X
Rule: X=XX[+XX]X[+XX]XX+
```

## 2. Square grammar puzzle
How about this one? Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

```
Angle: 90
Axiom: +X
Rule: X=X+X-X-X+X
```

## 3. Custom plant
My custom plant is as follows for several iterations (top: n = 2, 3, 4; bottom: n = 6, 7, 8):

<img width="200" src="https://github.com/user-attachments/assets/52b1f24b-0384-4206-9735-e769cd2adbe8">
<img width="200" src="https://github.com/user-attachments/assets/c8f6463e-c4ae-41e7-b518-6c1fd1548c18">
<img width="200" src="https://github.com/user-attachments/assets/eaf0d30c-b23d-4c16-bad7-c99bcbabc80f">
<br>
<img width="200" src="https://github.com/user-attachments/assets/5021e97c-1f1a-4d1b-8013-a57595aec998">
<img width="200" src="https://github.com/user-attachments/assets/90714578-3d08-452d-b081-0350f4920096">
<img width="200" src="https://github.com/user-attachments/assets/74e29f5b-d3a3-44f1-9c33-68c2c6bc59b2">

Using the following rules:
```
Angle; 20
Axiom: X
Rule1: X=X[-Y][-Y][+X]
Rule2: Y=FFY[F-F][+X]FX
```

The reference plant was thyme:

<img width="600" src="https://github.com/user-attachments/assets/1fba5754-432e-4d0c-aca0-2c3ee0b0d870">

I mainly attempted to imitate the stubbiness of the thyme leaves and how they branch in two directions from the stem.
I took creative liberty in the arrangement and growth of the stems themselves.

Rule 1 for `X` creates the arcing stem at the bottom of the plant.
From that stem, Rule 2 for `Y` is responsible for the branches of small and dense thyme leaves, as well as recursively creating new arcing stems for added complexity.
The plant at iterations n = 2, 3, 4 show how initially sparse the plant is. Notice how the bottom stem arcs as n increases, as well as how the branches from the stem grow.
The density of the leaves increases so that n = 6, 7 best match the reference image.
By n = 8, the plant has become so dense and complex that it achieves a wheat-like aesthetic.
