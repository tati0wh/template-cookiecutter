Como usar

data:
- raw: dados originais, NUNCA modificados
- interim: dados em processamento
- processed: dados prontos para modelagem
- external: dados que vieram de fontes externas

notebooks:
- notebooks exploratórios
- obs: colocar: 01_, 02_, 03,

src: guarda todo o código reutilizável
- data: funções para carregar/salvar dados
- features: criação de features
- models: código dos modelos
- visualization: funções de gráficos

models: modelos treinados


reports: relatórios ou figuras
------------------

Template para README

# Título

## Explicação

---

## Objetivo


---

## Estrutura de projeto

```
data-science-template/
│
├── data/
│   ├── raw/
│   ├── interim/
│   └── processed/
│
├── notebooks/
│
├── src/
│   ├── data/
│   ├── features/
│   ├── models/
│   └── visualization/
│
├── models/
├── reports/
│   └── figures/
│
├── README.md
├── requirements.txt
└── train.py

```

---

## Descrição dos Datasets

| File | Description |
|------|-------------|
| `train_churn_.csv` | Training dataset with labels |
| `test_churn_.csv` | Test dataset for submission |
| `sample_submission_.csv` | Submission format reference |

### Dicionário de dados

| Coluna | Descrição | Valores |
|---------|-------------|--------|


---

## Avaliação dos modelos

| Model | Accuracy | Precision | Recall | F1-Score | AUC-ROC |
|-------|----------|-----------|--------|----------|---------|
| Logistic Regression | - | - | - | - | - |
| Random Forest | - | - | - | - | - |
| XGBoost | - | - | - | - | - |
| **Best Model** | **-** | **-** | **-** | **-** | **-** |

> Veja [`models/model_results.md`](models/model_results.md) para análise detalhada dos modelos.

---

## Como rodar o repositório

### 1. Clonar o repositório
```bash
git clone https://github.com/your-username/customer-churn-prediction.git
cd customer-churn-prediction
```

### 2. Instalação de dependências
```bash
pip install -r requirements.txt
```

### 3. Rodar preprocessing.py e train.py
```bash
python src/preprocessing.py
python src/feature_engineering.py
python src/train.py
```

### 4. Ou explore os notebooks
```bash
jupyter notebook notebooks/01_eda.ipynb
```

---

## Tech Stack

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Wrangling-150458?style=flat&logo=pandas)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-F7931E?style=flat&logo=scikit-learn)
![XGBoost](https://img.shields.io/badge/XGBoost-Boosting-189fdd?style=flat)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-F37626?style=flat&logo=jupyter)

---

## Contexto

Esse projeto foi feito...

---

## Licensa

This project is open source and available under the [MIT License](LICENSE).
