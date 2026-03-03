# 🚀 Telecom X: Projeto de Análise de Evasão (Churn)

Este projeto foi desenvolvido como parte de um desafio de análise de dados para a empresa **Telecom X** <b>Alura + Oracle Next Education (ONE)</b>.. O objetivo principal é identificar os padrões que levam à evasão de clientes (Churn) e fornecer insights estratégicos para a retenção da base.

## 📋 Sobre o Projeto
A Telecom X enfrenta um alto índice de cancelamentos. Utilizando técnicas de **ETL** (Extração, Transformação e Carga) e **EDA** (Análise Exploratória de Dados), este projeto busca transformar dados brutos de uma API em informações acionáveis para as equipes de negócio e Data Science.

## 🛠️ Tecnologias Utilizadas
- **Linguagem:** Python 3.x
- **Bibliotecas:** - `Pandas`: Manipulação e tratamento de dados.
  - `Seaborn` & `Matplotlib`: Visualização de dados e criação de gráficos.
  - `Numpy`: Operações matemáticas e tratamento de nulos.
  - `JSON`: Processamento da fonte de dados original.

## 📉 Etapas do Desenvolvimento

### 1. Extração (Extract)
Leitura de dados brutos em formato JSON aninhado e conversão para DataFrame tabular utilizando `pd.json_normalize`.

### 2. Transformação (Transform)
- **Limpeza:** Remoção de dados nulos na variável alvo e tratamento de strings vazias.
- **Tipagem:** Conversão da coluna de faturamento total de texto para numérico.
- **Feature Engineering:** Criação da métrica `Gasto_Diario`.
- **Padronização:** Tradução de colunas para o Português e binarização de variáveis categóricas (Sim/Não para 1/0).

### 3. Análise Exploratória (EDA)
Identificação de métricas estatísticas e padrões visuais, como:
- Taxa global de churn de **26.5%**.
- Correlação entre contratos mensais e maior índice de cancelamento.
- Impacto do tempo de contrato (tenure) na fidelidade do cliente.

## 🔍 Principais Insights
- Clientes com **contratos mensais** são os mais propensos a sair.
- O risco de evasão é crítico nos **primeiros 12 meses** de relacionamento.
- Métodos de pagamento manuais (boleto/cheque eletrônico) possuem maior taxa de churn que os automáticos.

## 📂 Estrutura do Repositório
- `TelecomX_BR.ipynb`: Notebook principal com todo o código e relatório final.
- `TelecomX_Data.json`: Base de dados original utilizada.
- `TelecomX_dicionario.md`: Dicionário com a descrição das variáveis.

---
Desenvolvido por **Yasmin Caetano**
