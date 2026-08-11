# **A Comparative Study of Bias in Classification Models Trained on Dermatology Datasets**

This repository contains the code that carries out research to identify whether CNNs and Vision Transformers display equivalent amounts of bias when trained under identical conditions and on the same dataset.

Four models were trained and evaluated: **ResNet 50**, **DenseNet 121**, **ViT B/16**, and a **Swin Transformer**. The primary dataset utilized for the experiments was the **Fitzpatrick 17k**. Additionally, the **Stanford DDI** dataset was utilized to revalidate the findings on a second dataset.

## Repository Structure
```
├── fitzpatrick17k research/
├── DDI research/
├── requirements.txt
└── README.md
```
## Datasets used
**Fitzpatrick 17k** - (Groh et al., 2021), Link to the dataset-https://github.com/mattgroh/fitzpatrick17k.

**Standford DDI** - (Daneshjou et al., 2022), Link to the dataset-https://aimi.stanford.edu/datasets/ddi-diverse-dermatology-images

## Setup
```bash
git clone https://github.com/Akhilll321/Dissertation-code.git
cd Dissertation-code
pip install -r requirements.txt
```

## Steps to Run

```bash
python fitzpatrick17k_experiment.py
python ddi_experiment.py
```

Each of the script files handles all data preprocessing, loading, and training all four models, as well as obtaining the metrics and plots for bias evaluation for each of the datasets(Fitzpatrick 17k and Standford DDI ) 

## Acknowledgement

I would like to sincerely thank my supervisor, Dr David Harris-Birtill, for his invaluable support and insights throughout this project.



