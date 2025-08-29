# -Detec-o-de-Fraudes-Banc-rias
## 📌 Problema de Negócio Fraudes bancárias representam bilhões em perdas todos os anos, além de reduzirem a confiança do cliente nas instituições financeiras.   O objetivo deste projeto é **desenvolver um modelo de Machine Learning capaz de identificar transações fraudulentas com alta precisão**, reduzindo prejuízos e aumentando a segurança.
---

## 🎯 Objetivos
- Analisar padrões de transações financeiras.
- Tratar dados desbalanceados e garantir robustez do modelo.
- Testar diferentes algoritmos de classificação.
- Avaliar desempenho com validação cruzada.
- Gerar insights aplicáveis ao **contexto de negócios bancários**.

---

## 📂 Base de Dados
- **Fonte**: [Dataset de transações bancárias (Kaggle ou similar)]  
- **Tamanho**: XX mil registros, com variáveis como:
  - `amount` → valor da transação  
  - `time` → horário relativo  
  - `type` → tipo da transação  
  - `is_fraud` → variável alvo (fraude = 1, legítima = 0)

---

## 🔬 Metodologia
1. **Exploração e Análise de Dados (EDA)**  
   - Identificação de outliers  
   - Distribuição de classes (fraudes raras ≈ 0,2%)  
   - Correlação entre variáveis  

2. **Pré-processamento**  
   - Encoding de variáveis categóricas  
   - Normalização de valores monetários  
   - Balanceamento de classes (undersampling/oversampling)  

3. **Modelagem**  
   Algoritmos testados:
   - Logistic Regression  
   - Random Forest  
   - XGBoost  

4. **Validação**  
   - Uso de **StratifiedKFold Cross-Validation**  
   - Métricas: **Precision, Recall, F1-score e AUC**  

---

## 📊 Resultados
- **Melhor modelo**: XGBoost  
- **Métricas (exemplo, ajuste conforme seus resultados):**  
  - AUC: 0.97  
  - Precision: 0.91  
  - Recall: 0.88  
  - F1-Score: 0.89  

**Principais insights de negócio:**
- O modelo consegue identificar a maioria das transações fraudulentas.  
- Reduz falsos negativos → menos fraudes passam despercebidas.  
- Impacto: redução significativa de perdas financeiras + maior confiança dos clientes.  

---

## 🚀 Conclusões
- A aplicação de Machine Learning em fraudes bancárias é **viável e eficaz**.  
- O modelo pode ser integrado em sistemas de monitoramento em tempo real.  
- Além de prevenir perdas, fortalece a **imagem de segurança** da instituição.  

---

## 📈 Próximos Passos
- Testar algoritmos de Deep Learning (LSTM, Redes Neurais).  
- Implementar **detecção em tempo real** com streaming de dados.  
- Aplicar técnicas avançadas de **explainable AI (SHAP, LIME)** para auditoria e compliance.

- Instale as dependências

pip install -r requirements.txt
