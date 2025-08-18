# MedTrustAI
# 🏥 Healthcare Fraud Detection Project  

## 🇧🇷 Versão em Português  

### 📌 Meu Modelo Preditivo de Machine Learning  
Um modelo de ML preditivo para **detecção de anomalias e prevenção de fraudes em planos de saúde corporativos**.  
Combina análise de dados clínicos, temporais e financeiros com interpretabilidade baseada em **SHAP** e dashboards interativos para apoiar auditoria e tomada de decisão.  

---

### 💡 Gerador de Base Sintética de Fraudes em Saúde  

#### 🔎 Visão Geral  
Este projeto gera uma **base de dados sintética** de saúde, projetada para experimentos de detecção de fraudes usando Machine Learning.  
Ele simula **10.000 registros de atendimentos médicos** e injeta três tipos comuns de fraudes:  

- **Phantom Billing** – Serviços cobrados, mas não realizados.  
- **Upcoding** – Cobrança de procedimentos mais caros do que os realmente realizados.  
- **Duplicidade de Cobrança** – Cobrança repetida pelo mesmo serviço.  

A base contém dados de beneficiários, prestadores, serviços, diagnósticos, pagamentos e autorizações, tornando-a adequada para treinar e testar modelos de detecção de anomalias.  

---

#### ⚙️ Recursos  
✅ Gera dados realistas e estruturados de atendimentos médicos  
✅ Permite configurar a porcentagem de fraudes injetadas  
✅ Salva automaticamente o dataset em formato CSV  
✅ Pronto para uso em análise de dados e treinamento de modelos de ML  

---

#### 🛠️ Como Funciona  
1. **Criação dos Dados** – Gera aleatoriamente campos como `beneficiario_id`, `prestador_id`, `CID`, `tipo_atendimento` e `valor_pago`.  
2. **Injeção de Fraudes** – Introduz:  
   - Phantom Billing (data do serviço ausente)  
   - Upcoding (procedimentos de urgência desnecessários)  
   - Duplicidade de Cobrança (valores de pagamento anormalmente altos)  
3. **Exportação** – Salva como `banco_dados_sintetico_operadora.csv` e permite download via Google Colab.  

⚠️ **Importante**: Para a lógica do projeto funcionar corretamente, é necessário seguir os **passos 1–12** definidos na implementação.  

---

#### 📂 Estrutura de Arquivos  
📦 healthcare-fraud-generator
├── main.py # Código para gerar a base
├── banco_dados_sintetico_operadora.csv # Base de dados gerada
└── README.md # Documentação do projeto

yaml
Copiar
Editar

---

#### 🚀 Como Executar  
- Abra no **Google Colab** ou em qualquer ambiente Python.  
- Instale as dependências:  
  ```bash
  pip install pandas numpy
Execute o script.

Baixe o CSV gerado.

📊 Exemplo de Saída
id_atendimento	beneficiario_id	prestador_id	data_solicitacao	CID	valor_pago	procedimentos_urgencia
1	5432	456	2023-05-12	A00	512.50	nao

📜 Licença
Este projeto está licenciado sob a MIT License – livre para uso, modificação e distribuição.

🇬🇧 English Version
📌 My Predictive Machine Learning Model
A predictive ML model for anomaly detection and fraud prevention in corporate health plans.
It combines clinical, temporal, and financial data analysis with SHAP-based interpretability and interactive dashboards to support auditing and decision-making.

💡 Synthetic Healthcare Fraud Dataset Generator
🔎 Overview
This project generates a synthetic healthcare dataset designed for fraud detection experiments using Machine Learning.
It simulates 10,000 medical claim records and injects three common fraud types:

Phantom Billing – Services billed but not actually performed.

Upcoding – Billing for more expensive procedures than actually provided.

Duplicate Billing – Charging multiple times for the same service.

The dataset contains patient, provider, service, diagnosis, payment, and authorization details, making it suitable for training and testing anomaly detection models.

⚙️ Features
✅ Generates realistic, structured health claim data
✅ Configurable fraud injection percentages
✅ Automatically saves the dataset as CSV
✅ Ready to use for data analysis and ML model training

🛠️ How It Works
Data Creation – Randomly generates fields such as beneficiario_id, prestador_id, CID, tipo_atendimento, and valor_pago.

Fraud Injection – Introduces:

Phantom Billing (missing service date)

Upcoding (unnecessary urgent procedures)

Duplicate Billing (abnormally high payment values)

Export – Saves as banco_dados_sintetico_operadora.csv and allows download via Google Colab.

⚠️ Important: For the project logic to work correctly, it is necessary to follow steps 1–12 defined in the implementation.

📂 File Structure
bash
Copiar
Editar
📦 healthcare-fraud-generator  
 ├── main.py                              # Code to generate dataset  
 ├── banco_dados_sintetico_operadora.csv  # Generated dataset  
 └── README.md                            # Project documentation  
🚀 How to Run
Open in Google Colab or any Python environment.

Install dependencies:

bash
Copiar
Editar
pip install pandas numpy
Run the script.

Download the generated CSV.

📊 Example Output
id_atendimento	beneficiario_id	prestador_id	data_solicitacao	CID	valor_pago	procedimentos_urgencia
1	5432	456	2023-05-12	A00	512.50	nao

📜 License
This project is licensed under the MIT License – free to use, modify, and distribute.

