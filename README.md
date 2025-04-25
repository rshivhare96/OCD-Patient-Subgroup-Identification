# 🧠 OCD Patient Subgroup Identification

This project explores the segmentation of OCD (Obsessive-Compulsive Disorder) patients into distinct subgroups using **K-Means Clustering**. The dataset contains clinical, demographic, and symptom-related features aimed at uncovering patterns that can support **personalized clinical interventions** and deepen the understanding of OCD heterogeneity.

## 📊 Data

The dataset includes **clinical and demographic data** from OCD patients, with features such as:

- **Demographics**: Age, Gender, Ethnicity, Education Level, Marital Status  
- **Clinical History**: Duration of Symptoms, Comorbid Conditions (Anxiety, Depression), Family History, Medication Use  
- **Symptom Measures**: Obsession Severity, Compulsion Severity, Symptom Types

### Key Data Insights

- **Preprocessing** involved encoding categorical variables and scaling numerical features.
- **No significant missing values** after cleaning.
- Applied **dimensionality reduction (PCA)** for visualization and performance enhancement.
- **Elbow Method** determined the optimal number of clusters: **4**

## 🔍 Clustering Approach

Used **K-Means Clustering** to group patients into 4 subgroups based on combined demographic and clinical features.

### Cluster Characteristics

| Cluster | Age Range | Symptom Duration | Severity | Demographics | Clinical History         | Medications |
|---------|------------|------------------|----------|--------------|--------------------------|-------------|
| 0       | Mid-age    | Moderate         | Moderate | Mixed        | Some comorbidity         | Varies      |
| 1       | Younger    | Short            | High     | More males   | Fewer comorbid conditions| Less usage  |
| 2       | Older      | Long             | High     | More females | Strong family history    | High usage  |
| 3       | Mixed      | Variable         | Low      | Diverse      | Low comorbidity          | Low usage   |

> These clusters indicate real-world clinical variability and potential for personalized care strategies.

### Notable Findings

- **Obsession and compulsion scores** vary significantly across clusters.
- **Demographic factors** (like gender and education) influence cluster membership.
- **Medication use** and **symptom types** are distributed differently across subgroups.
- **Family and personal clinical history** patterns suggest differing etiologies and treatment needs.

## 📈 Visualizations

- PCA plots revealed clear **cluster separation** in reduced-dimensional space.
- Boxplots and heatmaps helped identify **feature-level differences** across clusters.

## 📁 Notebooks

- [`OCD_Clustering_Analysis.ipynb`](./OCD Patient Dataset Demographics & Clinical Data.ipynb): Full pipeline from preprocessing to clustering and insights.

## 📦 Requirements

Install required packages with:

```bash
pip install -r requirements.txt
