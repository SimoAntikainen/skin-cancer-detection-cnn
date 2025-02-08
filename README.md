# Skin Lesion Detection with InceptionV3  

Training scripts for **Deep Learning** model for **skin lesion classification**, leveraging **InceptionV3 with pretrained weights**. The model is trained on the **HAM10000 dataset** to detect **7 types of skin lesions**, aiding in early diagnosis.  

## Dataset  
We use the **HAM10000 dataset**, which consists of **10,000 dermatoscopic images** classified into **7 skin lesion types**.  

| Class Label | Description |
|------------|------------|
| **akiec**  | Actinic keratoses and intraepithelial carcinoma |
| **bcc**    | Basal cell carcinoma |
| **bkl**    | Benign keratosis-like lesions |
| **df**     | Dermatofibroma |
| **mel**    | Melanoma |
| **nv**     | Melanocytic nevi |
| **vasc**   | Vascular lesions |

🔗 **Data Source**: [HAM10000](https://www.kaggle.com/kmader/skin-cancer-mnist-ham10000)  


## Results
The model achieves an overall accuracy of 85%, demonstrating strong classification performance across seven skin lesion types.

## 🔹 Key Metrics  
| Metric            | Score |
|------------------|-------|
| **Micro Avg F1** | 0.85  |
| **Macro Avg F1** | 0.78  |
| **Weighted F1**  | 0.85  |

## 📊 Performance Breakdown by Class  
| Class  | Precision | Recall | F1-score | Support |
|--------|-----------|--------|----------|---------|
| **akiec** | 0.72  | 0.72  | 0.72  | 65  |
| **bcc**   | 0.76  | 0.87  | 0.81  | 103  |
| **bkl**   | 0.69  | 0.86  | 0.77  | 220  |
| **df**    | 0.71  | 0.87  | 0.78  | 23  |
| **mel**   | 0.55  | 0.58  | 0.56  | 223  |
| **nv**    | 0.95  | 0.89  | 0.92  | 1341  |
| **vasc**  | 1.00  | 0.75  | 0.86  | 28  |

## 🛠 Installation  
Ensure you have **Python 3.7+** and install dependencies using:  

```
conda env create -f environment.yml
or 

`pip install r -requirements.txt`

```

The scripts for training and visualization of the dataset are found in `train_inception.ipynb`
