# Desafio do titanic da plataforma kaggle

Este projeto tem como objetivo realizar **análise exploratória de dados (EDA)**, **limpeza e pré-processamento** e aplicar um modelo de **Machine Learning (Random Forest)** para prever a sobrevivência de passageiros do Titanic, utilizando o dataset clássico do Kaggle.

---

## 📊 Etapas do Projeto

1. **Carregamento dos Dados**
   - Dataset: `train.csv`
   - Fonte: [Kaggle - Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic)

2. **Análise Exploratória (EDA)**
   - Visualização dos primeiros registros
   - Estatísticas descritivas
   - Identificação de valores nulos
   - Distribuição de sobreviventes por sexo, classe social e idade
   - Gráficos com `matplotlib` e `plotly`

3. **Limpeza e Pré-processamento**
   - Remoção de colunas irrelevantes (`Cabin`, `Name`, `Ticket`, `Fare`, `PassengerId`)
   - Tratamento de valores nulos em `Age` (mediana) e `Embarked` (valor mais frequente)
   - Conversão de variáveis categóricas (`Sex`, `Embarked`)

4. **Modelagem**
   - Separação em variáveis independentes (X) e alvo (y)
   - Transformação do atributo `Survived` em classes (`Sobreviveu` / `Não sobreviveu`)
   - Treinamento de modelo com **RandomForestClassifier**
   - Avaliação com métricas: **acurácia, matriz de confusão e classification report**

---

## 🛠️ Tecnologias Utilizadas

- **Python 3.11**
- **Bibliotecas:**
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `plotly`
  - `scikit-learn`

---

## 📈 Principais Insights

- Mulheres tiveram maior taxa de sobrevivência em relação aos homens.
- Passageiros da **1ª classe** apresentaram maior chance de sobrevivência.
- Idade média dos sobreviventes variou conforme classe social e gênero.
- A variável `Cabin` foi descartada por conter mais de 77% de valores nulos.

---

## 🚀 Como Executar o Projeto

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/titanic-ml.git
   cd titanic-ml

