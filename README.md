# 📊 Análise de Churn - TelecomX

## 🎯 Objetivo
Este projeto realiza uma análise exploratória do **churn (cancelamento de clientes)** da TelecomX. O intuito é identificar os fatores mais relevantes para a evasão e gerar insights que ajudem a empresa a criar estratégias de retenção mais eficazes.

## 📂 Dados
- Fonte: [TelecomX_Data.json](https://raw.githubusercontent.com/ingridcristh/challenge2-data-science/refs/heads/main/TelecomX_Data.json)  
- Informações incluídas: dados demográficos, serviços contratados (telefone, internet, etc.), informações contratuais e cobranças.

## 🔎 Etapas da Análise
1. **Coleta** → Importação do arquivo JSON.  
2. **Preparação** → Expansão de colunas aninhadas, renomeação, tratamento de valores ausentes e criação de variáveis derivadas.  
3. **Exploração** → Análise da taxa de churn por perfil, contrato, serviços e pagamentos.  
4. **Visualização** → Gráficos ilustrativos (pizza, rosca, barras) para destacar padrões e tendências.  

## 📈 Principais Insights
- **Contratos Month-to-month** concentram a maior parte dos cancelamentos.  
- **Primeiros meses de uso** são os mais críticos para retenção.  
- Clientes de **fibra óptica** e pagamento via **Electronic check** apresentam maior propensão ao churn.  
- Usuários que cancelam pagam, em média, **valores mensais mais altos**.  

## ⚙️ Como Executar
Clone este repositório e instale as dependências necessárias, ou abra diretamente no **Google Colab**.  

### Requisitos
```bash
pip install pandas numpy matplotlib seaborn

