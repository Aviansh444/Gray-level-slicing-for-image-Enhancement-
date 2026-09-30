# Gray-level-slicing-for-image-Enhancement-

## Overview

Gray Level Slicing is an image enhancement technique used in Digital Image Processing to highlight a specific range of gray levels in an image. It helps emphasize important features while either preserving or suppressing the background.

This project implements two approaches:

1. **Gray Level Slicing Without Background**
2. **Gray Level Slicing With Background**

---

## Objective

* To enhance a selected range of gray levels in an image.
* To highlight specific image features based on pixel intensity.
* To compare slicing with and without background preservation.

---

## Technologies Used

* Python 3.x
* OpenCV
* NumPy
* Matplotlib

---

## Required Libraries

Install the required libraries using:

```bash
pip install opencv-python numpy matplotlib
```

---

## Project Structure

```text
Gray-Level-Slicing/
│
├── 23016CV05.py
├── 23016.jpg
├── README.md
└── Output
```

---

## Theory

Gray Level Slicing enhances pixels within a specified intensity range.

### Case 1: Without Background

Pixels within the selected range are assigned a high intensity value (255), while all other pixels are set to 0.

```text
If r1 ≤ pixel ≤ r2
    Output = 255
Else
    Output = 0
```

### Case 2: With Background

Pixels within the selected range are assigned a high intensity value (255), while the remaining pixels retain their original values.

```text
If r1 ≤ pixel ≤ r2
    Output = 255
Else
    Output = Original Pixel Value
```

---

## Algorithm

1. Read the grayscale image.
2. Define the gray-level range (`min_range` and `max_range`).
3. Create two output images:

   * With Background
   * Without Background
4. Traverse each pixel using nested loops.
5. Check whether the pixel intensity falls within the selected range.
6. Highlight selected pixels with intensity value 255.
7. Display the original and processed images.

---

## Input

A grayscale image:

```python
img = cv2.imread('/content/drive/MyDrive/COMPUTER VISION/23016.img', cv2.IMREAD_GRAYSCALE)
```

---

## Output

The program displays:

* Original Image
* Gray Level Slicing Without Background
* Gray Level Slicing With Background

```text
+-------------------+--------------------------+-----------------------+
| Original Image    | Without Background       | With Background       |
+-------------------+--------------------------+-----------------------+
```

---

## Applications

* Medical Image Analysis
* Defect Detection
* Satellite Image Processing
* Pattern Recognition
* Industrial Inspection
* Computer Vision Systems

---

## Learning Outcomes

After completing this project, you will be able to:

* Understand Gray Level Slicing.
* Enhance selected intensity ranges in images.
* Preserve or suppress image backgrounds.
* Apply image enhancement techniques in practical applications.

---

## Author

**Muvva Avinash*

B.Tech – Computer Science / Data Science

Computer Vision Laboratory
