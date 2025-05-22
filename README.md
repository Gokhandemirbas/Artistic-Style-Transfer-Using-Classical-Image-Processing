# 🎨 Artistic Style Transfer Using Classical Image Processing

This project implements artistic style transfer using only classical image processing techniques — without relying on any deep learning models such as VGG16.

All style transfer methods (HSV, Gabor, FFT, Canny, Sobel, Laplacian) are implemented inside a single notebook.

## 🧠 Objective

To transfer the stylistic color and texture features of a reference image onto a content image using techniques like histogram matching, edge detection, and frequency-based filters — while preserving structural content.

## 📄 Files in Repository

```
├── ArtisticStyleTransfer.ipynb   # Main notebook (all methods implemented here)
├── images.zip                    # Contains test style and content images
├── README.md                     # Project description and usage
```

## ⚙️ Included Methods

- Edge Detection: Canny, Sobel, Laplacian
- Style Encoding: HSV Histogram Matching, Gabor Texture Filters, FFT Phase Transfer
- Fusion: Combined via alpha blending with optional smoothing

## 📊 Evaluation Metrics

Two metrics were used for comparison:
- **SSIM**: Measures how well the structure of the content image is preserved.
- **HistSim**: Measures how well the color palette matches the style image using HSV histograms.

## 🏆 Results Summary

| Method       | SSIM        | HistSim     |
|--------------|-------------|-------------|
| HSV          | 0.711       | **0.979**   |
| Gabor        | 0.456       | 0.892       |
| FFT          | 0.050       | 0.327       |
| Canny        | 0.857       | 0.954       |
| Sobel        | 0.841       | 0.946       |
| Laplacian    | **0.874**   | 0.958       |

## 🚀 How to Run

1. Open the notebook `ArtisticStyleTransfer.ipynb` in Google Colab or Jupyter Notebook.
2. Upload your style and content images when prompted.
3. Select a method and view stylized results with evaluation scores.

## 📌 Credits

Based on classical image processing principles.  
Notebook inspired by:  
[Artistic Style Transfer - Udemy Notebook](https://github.com/ayyucekizrak/Udemy_DerinOgrenmeyeGiris/blob/master/Evrisimli_Sinir_Aglari/Artistik_Stil_Transferi/ArtistikStilTransferi.ipynb)

## 📚 Report

A full academic report is available as `style_transfer_report.docx`.

---

## 🧾 License

This project is for educational use only and is shared under the MIT License.
