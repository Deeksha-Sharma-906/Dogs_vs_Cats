# Dogs_vs_Cats_Classification
A deep learning model built with TensorFlow & Keras to classify images of dogs and cats using image data generators for training and validation.

# Dogs vs Cats Image Classification with TensorFlow  

## 📌 Project Overview  
This project demonstrates how a deep learning model built using **TensorFlow & Keras** can classify images of **dogs and cats**.  
The dataset comes from the popular **Kaggle Dogs vs Cats competition**, consisting of labeled images of two categories: dogs and cats.  

The model leverages **ImageDataGenerator** to preprocess, augment, and batch the image data, followed by training with validation monitoring to evaluate performance.  

---

## 🛠 Dataset: Dogs vs Cats  
- **Source:** Kaggle Dogs vs Cats dataset  
- **Size:** 25,000 images (12,500 dogs + 12,500 cats)  
- **Image Dimensions:** Resized (commonly to 150×150 or 224×224 pixels)  
- **Classes (2 categories):**  
  - 0️⃣ Cat  
  - 1️⃣ Dog  

---

## ⚙️ Approach  
1. **Data Preparation**  
   - Images are loaded using **ImageDataGenerator**  
   - Data is split into training and validation sets  
   - Rescaling and augmentation applied (normalization, flips, zoom, etc.)  

2. **Model Training**  
   - The model is trained with the prepared data using:  
     ```python
     model.fit(train_idg, batch_size=batch_size, epochs=10, validation_data=val_idg)
     ```
   - **Batch size** and **number of epochs** are adjustable hyperparameters  
   - **Validation data** monitors performance during training  

3. **Evaluation**  
   - Model accuracy and loss are tracked on both training and validation sets  
   - Post-training evaluation performed on the test dataset  

---

## 📊 Key Metrics  
- **Training Accuracy & Loss**  
- **Validation Accuracy & Loss**  
- Metrics can be visualized using accuracy/loss curves 
