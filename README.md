# which-bollywood-celebrity-are-you

A streamlit web app which can tell with which bollywood celebrity you face resembles

# !pip install mtcnn==0.1.0

# !pip install tensorflow==2.3.1

# !pip install keras==2.4.3

# !pip install keras-vggface==0.6

# !pip install keras_applications==1.0.8

# Required pkg for working

# Which Bollywood Celebrity Are You? 🎭

This project is a **Face Look-Alike Detection System** that matches a user's uploaded image with Bollywood celebrities and recommends the closest look-alike.

---

## 🚀 Project Overview

- Upload an image of any person.
- System detects the face using **MTCNN**.
- Extracts facial features using **VGGFace (ResNet50)**.
- Compares features with a precomputed dataset of Bollywood actors.
- Returns the celebrity with the **highest cosine similarity score**.

---

## 📂 Project Structure

```
├── dataset/             # Bollywood celebrity images
│   ├── actor1/
│   ├── actor2/
│   └── ...
├── uploads/             # User uploaded images
├── embedding.pkl        # Precomputed embeddings of celebrity faces
├── filenames.pkl        # File paths of celebrity dataset images
├── app.py               # Streamlit web app
├── feature_extract.py   # Code for feature extraction & embeddings
├── recommendation.py    # Code for similarity matching
├── requirements.txt     # Dependencies
└── README.md            # Project documentation
```

---

## ⚙️ Tech Stack

- **Python**
- **TensorFlow/Keras**
- **Keras-VGGFace**
- **MTCNN** (Face Detection)
- **OpenCV + PIL**
- **Scikit-learn**
- **Streamlit** (Web App)

---

## 📊 Workflow

1. Upload Image
2. Face Detection (MTCNN)
3. Feature Extraction (VGGFace - ResNet50)
4. Similarity Calculation (Cosine Similarity)
5. Best Match Celebrity is displayed

---

## 🔑 Key Features

- Celebrity face recognition using deep learning.
- Simple UI with Streamlit.
- Cosine similarity for closest match.
- Supports Bollywood dataset (can be extended).

---

## 🖼️ Results

- Uploaded image displayed on left.
- Predicted celebrity & their image displayed on right.
- Example: If you upload Virat Kohli's picture → It returns Virat Kohli as match.

---

## 📌 Challenges

- Performance depends on dataset quality.
- Side poses & poor lighting reduce accuracy.
- Computationally heavy for large datasets.

---

## 🚧 Future Improvements

- Add Top-3 predictions instead of single output.
- Extend dataset to Hollywood, sports, politics.
- Deploy model on **cloud (Heroku/Streamlit Cloud)** for public use.
- Train custom model for better accuracy.

---

## 📝 References

- [Keras VGGFace](https://github.com/rcmalli/keras-vggface)
- [MTCNN Face Detection](https://github.com/ipazc/mtcnn)
- [Streamlit Documentation](https://docs.streamlit.io/)
