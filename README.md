# MedTrustAI - 🏥 Healthcare Fraud Detection Project

## 🇧🇷 Versão em Português

### 📌 Meu Modelo Preditivo de Machine Learning
Modelo de ML preditivo para detecção de anomalias e prevenção de fraudes em planos de saúde corporativos.  
Combina análise de dados clínicos, temporais e financeiros com interpretabilidade baseada em SHAP e dashboards interativos para apoiar auditoria e tomada de decisão.

### 💡 Gerador de Base Sintética de Fraudes em Saúde

#### 🔎 Visão Geral
Este projeto gera uma base de dados sintética de saúde, projetada para experimentos de detecção de fraudes usando Machine Learning.  
Ele simula **10.000 registros de atendimentos médicos** e injeta três tipos comuns de fraudes:

- **Phantom Billing** – Serviços cobrados, mas não realizados.  
- **Upcoding** – Cobrança de procedimentos mais caros do que os realmente realizados.  
- **Duplicidade de Cobrança** – Cobrança repetida pelo mesmo serviço.  

A base contém dados de beneficiários, prestadores, serviços, diagnósticos, pagamentos e autorizações, tornando-a adequada para treinar e testar modelos de detecção de anomalias.

#### ⚙️ Recursos
✅ Gera dados realistas e estruturados de atendimentos médicos  
✅ Permite configurar a porcentagem de fraudes injetadas  
✅ Salva automaticamente o dataset em formato CSV  
✅ Pronto para uso em análise de dados e treinamento de modelos de ML  

#### 🛠️ Como Funciona: EM DESENVOLVIMENTO
⚠️ Importante: Para a lógica do projeto funcionar corretamente, é necessário seguir os **passos 1–12** definidos na implementação.

#### 📂 Estrutura de Arquivos: EM DESENVOLVIMENTO

### 🚀 Como Executar
- Abra no **Google Colab** ou em qualquer ambiente Python.  
- Execute o script.

### 🧰 Bibliotecas Utilizadas
- `pandas`, `numpy`, `random`, `datetime`  
- `sklearn.model_selection` (train_test_split)  
- `sklearn.preprocessing` (LabelEncoder)  
- `imblearn.over_sampling` (SMOTE)  
- `sklearn.ensemble` (RandomForestClassifier)  
- `shap` (interpretabilidade)  

### 🔹 Observação do DataFrame e Balanceamento com SMOTE
- Após geração da base sintética.
- Uma coluna de rótulo única (`fraude_tipo`) é criada com quatro classes:  
  `phantom_billing`, `upcoding`, `duplicidade_pagamento` e `regular`.  
- É aplicado **LabelEncoder** para codificar a coluna de classes.  
- As features (`X`) e o target (`y`) são separados.  
- **SMOTE** é aplicado para criar um dataset balanceado, garantindo aproximadamente **25% para cada classe**, pronto para treinamento.

### 🇧🇷 Treinamento e Avaliação do Modelo
- O dataset é dividido em **70% treino e 30% teste**.  
- O modelo utilizado é **Random Forest Classifier**, adequado para dados tabulares e classificação multiclasse.  
- Avaliação do modelo mostra **f1-score médio de 0.98**, indicando alta precisão na detecção de fraudes sintéticas.

### 📜 Licença
Este projeto está licenciado sob a MIT License – livre para uso, modificação e distribuição.

---

## 🇬🇧 English Version

### 📌 My Predictive Machine Learning Model
A predictive ML model for anomaly detection and fraud prevention in corporate health plans.  
It combines clinical, temporal, and financial data analysis with SHAP-based interpretability and interactive dashboards to support auditing and decision-making.

### 💡 Synthetic Healthcare Fraud Dataset Generator

#### 🔎 Overview
This project generates a synthetic healthcare dataset designed for fraud detection experiments using Machine Learning.  
It simulates **10,000 medical claim records** and injects three common fraud types:

- **Phantom Billing** – Services billed but not actually performed.  
- **Upcoding** – Billing for more expensive procedures than actually provided.  
- **Duplicate Billing** – Charging multiple times for the same service.  

The dataset contains information on patients, providers, services, diagnoses, payments, and authorizations, making it suitable for training and testing anomaly detection models.

#### ⚙️ Features
✅ Generates realistic and structured medical claim data  
✅ Allows configuration of fraud injection percentages  
✅ Automatically saves the dataset in CSV format  
✅ Ready to use for data analysis and ML model training  

#### 🛠️ How It Works: UNDER DEVELOPMENT
⚠️ Important: For the project logic to work correctly, it is necessary to follow the **steps 1–12** defined in the implementation.

#### 📂 File Structure: UNDER DEVELOPMENT

### 🚀 How to Run
- Open in **Google Colab** or any Python environment.  
- Run the script.

### 🧰 Libraries Used
- `pandas`, `numpy`, `random`, `datetime`  
- `sklearn.model_selection` (train_test_split)  
- `sklearn.preprocessing` (LabelEncoder)  
- `imblearn.over_sampling` (SMOTE)  
- `sklearn.ensemble` (RandomForestClassifier)  
- `shap` (interpretability)  

### 🔹 DataFrame Observation and SMOTE Balancing
- Generation of the synthetic dataset.
- A single label column (`fraude_tipo`) is created with four classes:  
  `phantom_billing`, `upcoding`, `duplicidade_pagamento`, and `regular`.  
- **LabelEncoder** is applied to encode the classes.  
- Features (`X`) and target (`y`) are separated.  
- **SMOTE** is applied to create a balanced dataset with approximately **25% for each class**, ready for model training.

### 🇬🇧 Model Training & Evaluation
- The dataset is split into **70% training and 30% testing**.  
- The model used is a **Random Forest Classifier**, suitable for tabular data and multiclass classification.  
- Model evaluation achieved an **average f1-score of 0.98**, indicating high accuracy in detecting synthetic frauds.

### 📜 License
This project is licensed under the MIT License – free to use, modify, and distribute.

