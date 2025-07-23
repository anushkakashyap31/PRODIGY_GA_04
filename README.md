> # **🚀 PRODIGY_GA_04 — Image-to-Image Translation using cGAN called Pix2Pix**

This repository contains **Task 4: Image-to-Image Translation Project** as part of my **Generative AI Internship at Prodigy Infotech**, where I implemented a Conditional GAN (cGAN) model called Pix2Pix for translating images from one domain to another (e.g., building edges to real buildings).


### **💡 Project Overview**

In this task, I have:

- Implemented a **Pix2Pix model** using TensorFlow and Keras.
- Trained a **conditional GAN** on the **facades dataset** (edge → photo).
- Generated high-quality images from sketch-style inputs.
- Worked on **Google Colab** using GPU for training and testing.

### **📄 Files**
- `Task4_pix2pix.ipynb`: Colab notebook with full implementation of the Pix2Pix pipeline.
Due to GitHub size limits, some files are stored externally:
- [🔗 Download pix2pix_generator_model.h5](https://drive.google.com/file/d/1G24H35qu0cjMcYdPRTg1hCYhP1U0yWeY/view?usp=sharing)
- [🔗 Download pix2pix_generator_model.keras](https://drive.google.com/file/d/11o2W3p_aXUlYB1KrX3WCJrr1Vln-qFbB/view?usp=sharing)
- [🔗 facades Dataset (Preprocessed)](https://drive.google.com/file/d/1k6VjFTZKp9-Qm6ALvUhAUF9fCnuNgT-6/view?usp=sharing)

### **⚙️ Technologies Used**

- Python
- Google Colab
- TensorFlow & Keras
- Matplotlib, NumPy
- Pix2Pix (Conditional GAN)

### **💬 How to Use**

1️⃣ Open the Notebook in Google Colab: [🔗][https://colab.research.google.com/drive/1_QoG9N5Pp9mpkGCDn3axE-3cMxzr4Zu0#scrollTo=gtleOVcswnwq]
Upload and open Task4_pix2pix.ipynb

2️⃣ Run All Cells Sequentially:
Includes the following steps:
  - Download and prepare dataset
  - Build Generator and Discriminator models
  - Define loss functions and optimizers
  - Train the Pix2Pix model
  - Visualize predictions

✅ Sample Inference:
```
# Load pre-trained generator
generator = tf.keras.models.load_model('pix2pix_generator_model.h5')

# Generate prediction from input image
prediction = generator(input_image, training=True)

# Display result
plt.imshow(prediction[0])

```

### **🎯 Objectives**

- Understand Conditional GANs and Pix2Pix architecture.
- Train an image-to-image translation model.
- Generate real-looking images from edge maps.

### **👩‍💻 Author**

### **Anushka Kashyap**

### **⭐ Acknowledgements**

- Prodigy Infotech
- Google Colab
- TensorFlow Team
- Original Pix2Pix Paper
- Facades Dataset (Berkeley)
**✨ Do ⭐ star the repo if you found it useful!**
