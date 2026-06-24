# AuraBloom 🌸

**AuraBloom** is a machine-learning and computer-vision system for **personal color analysis**.
From a user's photo, it extracts facial features — hair color, skin tone, and eye/undertone —
and uses them to determine the user's **seasonal color type**, recommend a matching color
palette (with a celebrity look-alike of the same season), and suggest suitable makeup.

This project was developed as a **graduation project** and showcases an end-to-end ML/CV
pipeline: face parsing, image-based color classification, clustering, and recommendation systems.

## ✨ Components

| Notebook | What it does | Key techniques |
|----------|--------------|----------------|
| `Hair_Color_Classificationa.ipynb` | Classifies hair color from a face image | FacePerceiver `facer` face parsing, `timm` |
| `SkinTone_Classification.ipynb` | Classifies skin tone from a face image | `facer` parsing, clustering (`pyclustering`) |
| `iris_vein_color_classification.ipynb` | Classifies eye color and warm/cool undertone | OpenCV, LAB color space, CIEDE2000 ΔE |
| `Seasonal_Color_Recommendation_System.ipynb` | Combines all features into a seasonal palette + celebrity match | Cosine similarity, one-hot encoding, `ipywidgets` |
| `Makeup_knowledge_recommender.ipynb` | Recommends makeup based on user features | One-hot encoding, cosine similarity |

## 🛠️ Tech Stack

- **Language:** Python (Jupyter / Google Colab notebooks)
- **Computer Vision:** [facer](https://github.com/FacePerceiver/facer), OpenCV, scikit-image
- **Machine Learning:** scikit-learn, timm, pyclustering
- **Data:** pandas, NumPy, matplotlib, ipywidgets

## 🚀 Getting Started

The notebooks were built in **Google Colab**. To run them:

1. Open a notebook in Jupyter or Colab.
2. Run the setup cells to install dependencies (e.g. `facer`, `timm`, `pyclustering`).
3. Provide the required dataset/image files where indicated.

## 👩‍💻 Authors

- **Taif Alharbi** — [@CallMeTaif](https://github.com/CallMeTaif)
- **Rama Alyoubi**
- **Yara Alshehri**
- **Albatul Alghamdi**
- **Rimas Alshehri**
- **Gharam Badroon**

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
