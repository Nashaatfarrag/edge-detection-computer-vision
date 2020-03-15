
#Edge detection

### Matlab Code : 
``` matlab
I = imread('circuit.tif');
J = edge(I);
figure;
imshow(I); 
firstDev = edge(J, 'prewitt');
figure;
imshow(firstDev);
secondDev = edge(J, 'log');
figure;
imshow(secondDev); 
cannyAlg = edge(J, 'canny');
figure;
imshow(cannyAlg);
```

#### original Photo
![](original.png)
#### Edge detection with first derivative: 
 ![](1stDerivative.png)
#### Edge detection using  Second derivative : 
![](2ndDerivative.png)

#### Edge detection using canny algorithm: 
![](canny.png)
I think edge detection using canny algorithm can give us a better result 
