# lab03-grammars
## Zhen Ren

## 1. Wheat grammar puzzle
\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

### Solution: `F=FF[+F]F[+F]F+`
![](./wheat.png)

## 2. Square grammar puzzle
\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

### Solution: `F=F-F+F+F-F`
![](./square.png)

## 3. Acacia Tree
![](./acaciaImg.jpg)
The goal is to mimic an acacia tree. The main challenge is to make a flatten top with random branches. Therefore, I used different conditions to restrct the growth when the y coordinate is above certain threshold and when the arc length is greater than certain value.

![](./acacia.png)