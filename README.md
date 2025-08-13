# MedTrustAI
My Predictive Machine Learning model for anomaly detection and fraud prevention in corporate health plans. Combines clinical, temporal, and financial data analysis with SHAP-based interpretability and interactive dashboards to support auditing and decision-making.

Synthetic Healthcare Fraud Dataset Generator
📌 Overview
This project generates a synthetic healthcare dataset designed for fraud detection experiments using Machine Learning.
It simulates 10,000 medical claim records and injects three common fraud types:

Phantom Billing – Services billed but not actually performed.

Upcoding – Billing for more expensive procedures than actually provided.

Duplicate Billing – Charging multiple times for the same service.

The dataset contains patient, provider, service, diagnosis, payment, and authorization details, making it suitable for training and testing anomaly detection models.

⚙️ Features
Generates realistic, structured health claim data.

Configurable fraud injection percentages.

Automatically saves the dataset as CSV.

Ready to use for data analysis and ML model training.

🛠️ How It Works
Data Creation – Randomly generates fields such as beneficiario_id, prestador_id, CID, tipo_atendimento, and valor_pago.

Fraud Injection – Introduces:

Phantom Billing (missing service date)

Upcoding (unnecessary urgent procedures)

Duplicate Billing (abnormally high payment values)

Export – Saves as banco_dados_sintetico_operadora.csv and allows download via Google Colab.

📂 File Structure
bash
Copiar
Editar
📦 healthcare-fraud-generator
 ├── main.py  # Code to generate dataset
 ├── banco_dados_sintetico_operadora.csv  # Generated dataset
 └── README.md  # Project documentation
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
id_atendimento	beneficiario_id	prestador_id	data_solicitacao	CID_	valor_pago	procedimentos_urgencia
1	5432	456	2023-05-12	A00	512.50	nao

📜 License
This project is licensed under the MIT License – free to use, modify, and distribute.

