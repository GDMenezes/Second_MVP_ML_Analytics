# 📦 Previsão de Demanda - Projeto de Machine Learning

Este projeto tem como objetivo aplicar técnicas de regressão para prever a demanda de produtos em uma empresa fictícia do setor de bens de consumo. A simulação foi construída com base em situações reais enfrentadas por empresas que operam no modelo *Make to Stock*.

---

## 🧩 Descrição do Problema

A empresa **Well Being**, que atua no setor de cuidados pessoais (higiênicos, papel toalha, fraldas e guardanapos), tem enfrentado desafios com **estoques excessivos**, tanto de produtos acabados quanto de insumos. 

O gerente de logística solicitou uma análise dos pedidos de 2024 para orientar decisões estratégicas para 2025, com foco na **redução de estoques**, **ajuste de lead time** e **diminuição dos custos logísticos e industriais**.

---

## 🔍 Tipo de Problema

Este é um problema de **regressão supervisionada**, voltado para prever valores numéricos (quantidade de vendas), a partir de dados históricos e variáveis categóricas. Embora fosse possível utilizar modelos de séries temporais (*forecasting*), foi escolhido o uso de **modelos de regressão**, conforme explorado na disciplina.

---

## 📊 Construção do Dataset

Não foi encontrado um dataset público que representasse bem o problema real da área de logística. Por isso, foi decidido:

- **Criar diretrizes** com base na experiência prática.
- Utilizar o **ChatGPT** para gerar um dataset sintético seguindo essas diretrizes.
- Ajustar o dataset para torná-lo mais realista e aplicável ao modelo de previsão.

---

## 📁 Atributos do Dataset

O dataset `industria_consumo_data.csv` contém **392.830 amostras** e os seguintes **6 atributos**:

| Atributo           | Descrição                                                                 |
|--------------------|---------------------------------------------------------------------------|
| `Data_de_Venda`    | Data em que a venda foi realizada                                         |
| `Nome_do_Produto`  | Código/SKU do produto vendido                                             |
| `Quantidade_Vendida` | Quantidade de itens vendidos                                             |
| `Preço_Unitário`   | Preço de venda por unidade do produto                                     |
| `Região_de_Venda`  | Região geográfica da venda (ex: Sudeste, Sul, etc.)                       |
| `Promoção_Ativa`   | Indica se o produto estava com promoção no momento da venda (Sim/Não)     |

---

## 🧠 Abordagem e Metodologia

- Pré-processamento de dados
- Codificação de variáveis categóricas (Label Encoding)
- Divisão entre dados de treino e teste
- Treinamento de modelos de regressão
- Avaliação do desempenho (ex: MSE, RMSE)

> Também foi testado o uso de One-Hot Encoding, mas optou-se pelo Label Encoding por oferecer resultados similares com menor tempo de processamento.

---

## ✅ Resultados

O modelo de regressão foi capaz de prever a demanda com boa acurácia, permitindo:

- Otimização do controle de estoque
- Melhoria no planejamento logístico
- Redução de custos com armazenagem e produção
- Suporte à tomada de decisões estratégicas

---

## 🛠️ Tecnologias Utilizadas

- Python 3.10+
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn
- Jupyter Notebook

---

## 👨‍💻 Autor

Desenvolvido por Gabriel Silva Menezes como parte da disciplina de Machine Learning e Analytics.

---

## 💻 Executar no Google Colab

Clique no botão abaixo para abrir o notebook diretamente no Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/GDMenezes/Second_MVP_ML_Analytics/blob/main/MVP_ML_%26_Analytics.ipynb)
