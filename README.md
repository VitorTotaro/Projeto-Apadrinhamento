# 🇧🇷 Previsão de Preços de Diárias do Airbnb - Rio de Janeiro

## 🌟 Visão Geral do Projeto

Este projeto de Ciência de Dados e Machine Learning (ML) tem como objetivo **prever o preço ideal das diárias** de aluguéis por temporada no Rio de Janeiro (RJ), utilizando dados públicos da plataforma Airbnb.

O foco é aplicar técnicas de **Regressão** e **Análise Exploratória de Dados (EDA)** para identificar quais características de um imóvel (localização, tamanho, tipo de quarto e avaliações) mais influenciam no seu valor.

### 🎯 Objetivo Principal

Construir um modelo de Machine Learning capaz de estimar o preço da diária (`price`) de um imóvel com a maior precisão possível.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python
* **Análise e Manipulação de Dados:** `Pandas`, `NumPy`
* **Visualização de Dados:** `Matplotlib`, `Seaborn`, **`Plotly`** ou **`Folium`** (para mapas interativos)
* **Machine Learning (Regressão):** `Scikit-learn` (Modelos como Regressão Linear, Árvore de Decisão, ou Random Forest).

## 📊 Dados

Os dados utilizados neste projeto são públicos, fornecidos pelo [Inside Airbnb](http://insideairbnb.com/get-the-data/), e se referem às listagens de imóveis no Rio de Janeiro.

* **Principal Dataset:** `listings.csv` (Informações e métricas por imóvel).
* **Dataset Auxiliar:** `neighbourhoods.geojson` (Dados geográficos para visualização).

## 🔑 Principais Etapas do Projeto

1.  **Obtenção e Limpeza de Dados:** Carregamento dos dados do `listings.csv`, tratamento de valores nulos (dados faltantes) e remoção de *outliers* (preços muito discrepantes).
2.  **Análise Exploratória de Dados (EDA):**
    * Distribuição da variável alvo (`price`).
    * Identificação das correlações entre as características (e.g., tipo de quarto vs. preço).
3.  **Visualização Chamativa:**
    * Criação de **mapas interativos** mostrando o preço médio das diárias por bairro no Rio de Janeiro (usando latitude/longitude e o arquivo GeoJSON).
    * Gráficos da distribuição de preços por tipo de quarto (`room_type`).
4.  **Pré-processamento para ML:** Conversão de variáveis categóricas (como nomes de bairros) em formato numérico.
5.  **Modelagem e Treinamento:** Treinamento de um modelo de Regressão (ex: Regressão Linear Simples para o calouro, seguido de um Random Forest para melhoria).
6.  **Avaliação:** Medição do desempenho do modelo utilizando métricas como o Erro Médio Absoluto (MAE) e o R-quadrado ($R^2$).

## 💡 Ideias para próximos Passos (Evolução do Projeto se possível)

* **Aprofundamento em NLP:** Análise de sentimento nas colunas de descrição dos imóveis para ver como o texto influencia o preço.
* **Interface Web:** Criação de um pequeno aplicativo (usando **Streamlit** ou **Gradio**) onde o usuário pode inserir características de um imóvel e receber a previsão de preço.

---
*Desenvolvido por: Vitor Totaro Fialho e Felipe Anastasia*
