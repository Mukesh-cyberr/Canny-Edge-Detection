## Aim

To detect the edges present in an image using the Canny Edge Detection algorithm in OpenCV.

## Algorithm
1. Start the program.
2. Import the required libraries (cv2 and matplotlib).
3. Read the input image.
4. Convert the image to grayscale.
5. Apply the Canny edge detector with suitable threshold values.
6. Display the original image and the detected edges.
7. Stop the program.
## Program (Python)

```
import cv2
import matplotlib.pyplot as plt

img = cv2.imread("C:\\Users\\admin\\Downloads\\photo.jpeg",cv2.IMREAD_GRAYSCALE)

blurred =cv2.GaussianBlur(img, (5,5),0)

edges = cv2.Canny(blurred, 50, 150)


import matplotlib.pyplot as plt
plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
print("Mukesh Raj D")
print("212224100038")
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()
```
# Output
## Original Image

<img width="368" height="489" alt="image" src="https://github.com/user-attachments/assets/eb803147-95a5-4b92-b062-f325130011de" />

## Edge Detected Image

<img width="312" height="430" alt="image" src="https://github.com/user-attachments/assets/f02f8cce-f380-4112-b5ef-f1952e7443e1" />


## Result

Thus, the edges present in the given image were successfully detected using the Canny Edge Detection algorithm in OpenCV.
