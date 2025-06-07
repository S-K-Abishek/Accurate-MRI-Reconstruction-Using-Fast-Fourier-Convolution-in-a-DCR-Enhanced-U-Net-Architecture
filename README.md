
# Accurate MRI Image Reconstruction Using a Fast Fourier Convolution Layer within a DCR-Enhanced U-Net Architecture

## ⭐ Overview
This project presents a novel deep learning architecture that enhances MRI image reconstruction accuracy by integrating **Fast Fourier Convolution (FFC)** layers within **Densely Connected Residual (DCR)** blocks inside a U-Net architecture. The model efficiently captures **global spectral features** while reducing reconstruction artifacts and computational cost, making it highly suitable for **real-time clinical applications**.

---

## 🧠 Key Features

- ✔️ Combines spectral-domain learning (FFC) with spatial-domain learning (DCR).
- ✔️ Built on a U-Net backbone with improved skip connections and dense feature reuse.
- ✔️ Achieves superior **PSNR**, **SSIM**, and reduced **MSE** and **inference time** over conventional models.

---

## 🩻 Problem Statement
MRI is a critical imaging modality for diagnosing internal body structures. However, its **slow acquisition speed**, **high noise sensitivity**, and **computational burden** hinder clinical efficiency. This project aims to solve these challenges by proposing a **hybrid deep learning model** that improves the **quality and speed** of MRI reconstruction.

---

## 🔬 Scope
- Reconstruct **high-quality, low-noise MRI images** from noisy or incomplete data.
- Reduce computational load and inference time.
- Adaptable to different imaging modalities (e.g., brain and knee MRIs).

---

## 📂 Dataset

- **Source:** [NITRC - Neuroimaging Tools and Resources Collaboratory](https://www.nitrc.org/frs/?group_id=899)
- **Dataset:** 36 T1-weighted 3T Brain MRI Volumes
- **Format:** `.nii` (NIfTI)

---

## 🛠️ Technologies Used

- **Language:** Python
- **Libraries:** PyTorch, NumPy, Matplotlib, scikit-learn
- **Optimization:** RMSprop
- **Frameworks:** FFTConv2D-based convolution implementation

---

## ⚙️ System Configuration

- **Processor:** AMD Ryzen 7 5800HS with Radeon Graphics, 3.20 GHz, 8 Core(s), 16 Thread(s) 
- **RAM:** 16 GB  
- **GPU:** NVIDIA GeForce RTX 3050 Laptop GPU, 4 GB GDDR6 VRAM
- **Storage:** 1 TB SSD  
- **Software:** PyTorch 2.6.0, CUDA 12.6

---

## 🧪 Model Architecture

- **Encoder-Decoder** U-Net with skip connections
- Integrated **FFC layers** for frequency-domain operations
- Embedded **DCR blocks** for better gradient flow and feature reuse
- Final reconstruction using Sigmoid activation

## 📊 Visuals

![Input 3D image](https://raw.githubusercontent.com/S-K-Abishek/Accurate-MRI-Reconstruction-Using-Fast-Fourier-Convolution-in-a-DCR-Enhanced-U-Net-Architecture/main/Output/3D.png)

![3D to 2D image](https://raw.githubusercontent.com/S-K-Abishek/Accurate-MRI-Reconstruction-Using-Fast-Fourier-Convolution-in-a-DCR-Enhanced-U-Net-Architecture/main/Output/Data.jpg)

![System Design](https://raw.githubusercontent.com/S-K-Abishek/Accurate-MRI-Reconstruction-Using-Fast-Fourier-Convolution-in-a-DCR-Enhanced-U-Net-Architecture/main/Output/System%20Design.jpg)

![FFC-DCR Block Architecture](https://raw.githubusercontent.com/S-K-Abishek/Accurate-MRI-Reconstruction-Using-Fast-Fourier-Convolution-in-a-DCR-Enhanced-U-Net-Architecture/main/Output/DCR%20archictecture.png)

![Noisy Input](https://raw.githubusercontent.com/S-K-Abishek/Accurate-MRI-Reconstruction-Using-Fast-Fourier-Convolution-in-a-DCR-Enhanced-U-Net-Architecture/main/Output/Noisy%20CNN%20with%20DCR%20input.jpg)

![Reconstructed Output](https://raw.githubusercontent.com/S-K-Abishek/Accurate-MRI-Reconstruction-Using-Fast-Fourier-Convolution-in-a-DCR-Enhanced-U-Net-Architecture/main/Output/NOisy%20unet%20with%20dcr%20result.jpg)

![Qualitative Metrics](https://raw.githubusercontent.com/S-K-Abishek/Accurate-MRI-Reconstruction-Using-Fast-Fourier-Convolution-in-a-DCR-Enhanced-U-Net-Architecture/main/Output/Final%20Comparitive%20study.jpg)





### Input 3D image
![App Screenshot](https://github.com/S-K-Abishek/Accurate-MRI-Reconstruction-Using-Fast-Fourier-Convolution-in-a-DCR-Enhanced-U-Net-Architecture/blob/master/Output/3D.png?raw=true)

### 3D to 2D image
![App Screenshot](https://github.com/S-K-Abishek/Accurate-MRI-Reconstruction-Using-Fast-Fourier-Convolution-in-a-DCR-Enhanced-U-Net-Architecture/blob/master/Output/Data.jpg?raw=true)

### System Design  
![System Design](https://github.com/S-K-Abishek/Accurate-MRI-Reconstruction-Using-Fast-Fourier-Convolution-in-a-DCR-Enhanced-U-Net-Architecture/blob/master/Output/System%20Design.jpg?raw=true)

### FFC-DCR Block Architecture  
![DCR Architecture](https://github.com/S-K-Abishek/Accurate-MRI-Reconstruction-Using-Fast-Fourier-Convolution-in-a-DCR-Enhanced-U-Net-Architecture/blob/master/Output/FFC-DCR%20archictecture.png?raw=true)

### Noisy Input vs Reconstructed Output  
**Input**  
![Noisy Input](https://github.com/S-K-Abishek/Accurate-MRI-Reconstruction-Using-Fast-Fourier-Convolution-in-a-DCR-Enhanced-U-Net-Architecture/blob/master/Output/Noisy%20Input.jpg?raw=true)

**Output**  
![Reconstructed Output](https://github.com/S-K-Abishek/Accurate-MRI-Reconstruction-Using-Fast-Fourier-Convolution-in-a-DCR-Enhanced-U-Net-Architecture/blob/master/Output/Noisy%20output.jpg?raw=true)

## Qualitative Metrics
The qualitative metrics (PSNR - Peak Signal To Noise Ratio, SSIM - Structural Similarity Index, MSE - Mean Squared Error, and Inference Time) obtained with each model are presented in this section:
![Qualitative Metrics](https://github.com/S-K-Abishek/Accurate-MRI-Reconstruction-Using-Fast-Fourier-Convolution-in-a-DCR-Enhanced-U-Net-Architecture/blob/master/Output/Final%20Comparitive%20study.jpg?raw=true)

---

## 🚀 Future Enhancements

- Incorporate **adversarial loss** (GAN-based refinement)
- Extend to **3D MRI reconstruction**
- Apply to other modalities (CT, PET)
- Integrate **wavelet-based features** alongside Fourier features

---

## 📄 Published Paper

You can read the full paper published in IRJMETS here:  
🔗 [IRJMETS Publication (April 2025)](https://www.irjmets.com/uploadedfiles/paper//issue_4_april_2025/74233/final/fin_irjmets1746586232.pdf)

---

## 🤝 Authors

- [Abishek S K](https://github.com/S-K-Abishek)
- [Roshan Bosco A](mailto:ra1236@srmist.edu.in)
- [Vishal Yadav H](mailto:vh5329@srmist.edu.in)

---

## 📫 Feedback
If you have suggestions or feedback, feel free to reach out:  
📧 **shekabi626210@gmail.com**
