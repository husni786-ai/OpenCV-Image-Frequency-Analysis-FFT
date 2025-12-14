# 📉 Image Frequency Analysis with Fast Fourier Transform (FFT)

This project contains a Jupyter Notebook that demonstrates how to analyze and visualize the frequency domain of an image using the **Fast Fourier Transform (FFT)** within the **OpenCV (cv2)** and **NumPy** libraries. Understanding the frequency domain is crucial for tasks like image compression, noise filtering, and edge detection.

---

## 🎯 Project Goals

The objective is to implement a complete pipeline for transforming an image from the spatial domain (pixels) to the frequency domain and back:

1.  **Preparation:** Load a grayscale image and convert it to floating-point representation.
2.  **FFT Calculation:** Apply the 2D Discrete Fourier Transform (DFT) using NumPy's efficient FFT implementation.
3.  **Visualization:** Shift the zero-frequency component to the center and compute the magnitude spectrum (logarithmically scaled) for visualization. 
4.  **Inverse FFT (I-FFT):** Demonstrate how to reconstruct the original image from the magnitude and phase information in the frequency domain.

## ⚙️ Technology Stack and Dependencies

The project relies on standard Python libraries for scientific computing and computer vision:

| Library | Role |
| :--- | :--- |
| **`opencv-python (cv2)`** | Used for loading and displaying images. |
| **`numpy`** | Essential for performing the mathematical operations of the Fast Fourier Transform (`np.fft.fft2`, `np.fft.ifft2`, `np.fft.fftshift`). |
| **`matplotlib.pyplot`** | Used for visualizing the original image, the frequency spectrum, and the reconstructed image. |

### Installation

```bash
pip install opencv-python numpy matplotlib
