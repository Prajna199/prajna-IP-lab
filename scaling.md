```python
import numpy as np
import cv2 as cv
from  matplotlib import pyplot as plt
```


```python
#scaling
img = cv.imread('flower.jpg')

res = cv.resize(img,None,fx=2, fy=2, interpolation = cv.INTER_CUBIC)

```


```python
cv.imshow('img',res)
cv.imshow("original pic",img)
cv.imshow("resized pic",res)
cv.waitKey(0)
cv.destroyAllWindows()

```


```python
#affine transformtion
img = cv.imread('rose.jpg')
rows,cols,ch = img.shape
pts1 = np.float32([[50,50],[200,50],[50,200]])
pts2 = np.float32([[10,100],[200,50],[100,250]])
M = cv.getAffineTransform(pts1,pts2)
res = cv.warpAffine(img,M,(cols,rows))
plt.subplot(121),plt.imshow(img),plt.title('Input')
plt.subplot(122),plt.imshow(dst),plt.title('Output')
plt.show()
```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```
