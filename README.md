# 📊 Projeto de Previsão de Evasão Bancária (Churn)

Este repositório apresenta um estudo sobre **evasão bancária (churn)**, utilizando **Machine Learning** para prever quais clientes possuem maior probabilidade de sair do banco. O objetivo é identificar padrões e fatores que influenciam essa decisão.

---

## 📌 Objetivo

O objetivo principal deste projeto é construir um modelo preditivo capaz de identificar **clientes propensos a encerrar suas contas bancárias**. Para isso, são utilizadas técnicas de **análise exploratória**, **tratamento de dados**, **engenharia de features** e **aprendizado de máquina**.

---

## 🔎 Dados Utilizados

O conjunto de dados utilizado foi obtido a partir do repositório [Cassius F](https://github.com/cassiusf/datasets). Ele contém informações sobre clientes bancários, incluindo:

- **Credit Score** (Score de crédito do cliente)
- **Geography** (País de residência)
- **Gender** (Gênero do cliente)
- **Age** (Idade do cliente)
- **Tenure** (Tempo de relacionamento com o banco)
- **Balance** (Saldo da conta bancária)
- **NumOfProducts** (Quantidade de produtos bancários utilizados)
- **HasCrCard** (Se o cliente possui cartão de crédito ou não)
- **IsActiveMember** (Se é um membro ativo do banco)
- **EstimatedSalary** (Salário estimado)
- **Exited** (Se o cliente saiu do banco ou não) *(Variável alvo)*

---

## 🛠️ Técnicas Utilizadas

O projeto seguiu um fluxo padrão de aprendizado de máquina:

### 1️⃣ **Exploração dos Dados (EDA)**

- Análise de distribuição das variáveis
- Identificação de valores ausentes
- Remoção de colunas irrelevantes (*CustomerId*, *Surname*)

### 2️⃣ **Pré-processamento e Engenharia de Features**

- **Tratamento de valores nulos** (remoção de registros com valores ausentes)
- **Codificação de variáveis categóricas** (One-Hot Encoding para *Geography* e *Gender*)
- **Normalização de variáveis numéricas** usando *StandardScaler*
- **Identificação de outliers** por meio de *Boxplots*

### 3️⃣ **Divisão do Conjunto de Dados**

- Utilização do *train\_test\_split* para separar dados de treino e teste (*70% treino, 30% teste*)

### 4️⃣ **Tratamento de Desbalanceamento**

- Utilização do **SMOTE** (*Synthetic Minority Over-sampling Technique*) para balancear a classe alvo

### 5️⃣ **Treinamento de Modelos de Machine Learning**

- **Random Forest Classifier** para previsão da evasão
- Ajuste de hiperparâmetros para otimização do modelo

### 6️⃣ **Avaliação do Modelo**

- **Métricas Utilizadas:**
  - Acurácia
  - Precision, Recall e F1-score
  - Matriz de confusão
  - Curva ROC e AUC

---

## 🔧 Ferramentas e Bibliotecas Utilizadas

O projeto foi desenvolvido em **Python** e utiliza as seguintes bibliotecas:

- `pandas` → Manipulação e análise de dados
- `numpy` → Cálculos matemáticos
- `matplotlib` e `seaborn` → Visualização de dados
- `scikit-learn` → Modelagem e avaliação de Machine Learning
- `imblearn` → Tratamento de desbalanceamento com SMOTE

---


## 🚀 Como Executar o Projeto

1. Clone o repositório:
   ```bash
   git clone https://github.com/araujojv/projeto_evasao_bancaria.git
   cd projeto_evasao_bancaria
   ```
2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
3. Execute o Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Abra e rode o notebook `evasao.ipynb`.

---

## 📌

## &#x20;Contribuição

Sinta-se à vontade para contribuir com o projeto abrindo **issues** ou enviando **pull requests**. Sugestões para novas técnicas e otimizações são bem-vindas!

---

✍️ **Autor:** [@araujojv](https://github.com/araujojv)

