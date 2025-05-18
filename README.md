# imageProcessing
# Image Processing Transformations

This project demonstrates the application of several fundamental image processing techniques using Python and OpenCV. The transformations applied include:

- Cropping
- Affine Transformation
- Grayscale Conversion
- Log Transformation
- Gamma Correction

## 📌 Overview

The purpose of this project is to understand how basic image transformation operations affect image appearance and structure. It serves as a useful tool for beginners in computer vision or image preprocessing pipelines in machine learning.

---

## 🛠️ Technologies Used

- Python 3.x
- OpenCV
- NumPy
- Matplotlib (optional for visualization)



## 🔄 Transformations Explained

### ✅ Cropping
Extract a region of interest from the image.

```python
cropped_img = image[y:y+h, x:x+w]
```

---

### ✅ Affine Transformation
Apply rotation, translation, or scaling to the image using an affine matrix.

```python
cv2.warpAffine(image, matrix, (width, height))
```

---

### ✅ Grayscale Conversion
Convert the image from RGB to grayscale.

```python
gray_img = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
```

---

### ✅ Log Transformation
Enhance details in darker areas by applying logarithmic scaling.

```python
log_img = c * np.log1p(gray_img)
```

---

### ✅ Gamma Correction
Adjust image brightness non-linearly.

```python
gamma_corrected = np.power(image / 255.0, gamma) * 255
```

---
### CONCLUSION
This project provides a hands-on understanding of basic image processing techniques using Python and OpenCV. By applying transformations such as cropping, affine changes, grayscale conversion, log transformation, and gamma correction, users gain insight into how these methods affect visual data. This foundational knowledge is essential for further exploration in computer vision, machine learning, and digital image analysis.
