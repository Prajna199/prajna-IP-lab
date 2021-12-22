```python

import cv2
import numpy as np
import matplotlib.pyplot as plt

```


```python
img= cv2.imread('gas1.jpg')

cv2.imshow("Images",img)
cv2.waitKey(0)
cv2.destroyAllWindows()

```


```python
gray_img=cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)

```


```python
gray_img_eqhist=cv2.equalizeHist(gray_img)
hist=cv2.calcHist(gray_img_eqhist,[0],None,[256],[0,126])

```


```python
cv2.imshow("Images",gray_img_eqhist)
cv2.waitKey(0)
cv2.destroyAllWindows()
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
