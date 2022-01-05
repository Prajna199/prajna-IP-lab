# prajna-IP-lab
1.Develop a program to perform linear transformation on the image.

 Description:
 import cv2
image = cv2.imread('girl.jpg')
height, width = image.shape[:2]
center = (width/2, height/2)
rotate_matrix = cv2.getRotationMatrix2D(center=center, angle=60, scale=1)
rotated_image = cv2.warpAffine(src=image, M=rotate_matrix, dsize=(width, height))
cv2.imshow('Original image', image)
cv2.imshow('Rotated image', rotated_image)
cv2.waitKey(0)
cv2.imwrite('rotated_image.jpg', rotated_image)

![image](https://user-images.githubusercontent.com/95853471/148199172-6c51b81e-3fa0-4f87-9c37-5361d8173cee.png)
