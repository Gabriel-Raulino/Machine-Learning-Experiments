# 📊 Supervised Machine Learning: Classification & Regression

<details>
<summary>🇺🇸 <b>Read in English</b></summary>
<br>

This repository contains academic experiments developed for the Artificial Intelligence course at UFSC. The project focuses on the practical application of Classical Machine Learning algorithms using `scikit-learn` to solve two distinct real-world problems: Multiclass Classification and Continuous Regression.

### 🎯 Project Objectives & Datasets

#### 1. Multiclass Classification: Brazilian Football Championship
*   **Dataset:** Historical data of the Brazilian Football Championship (Campeonato Brasileiro).
*   **Target Variable:** Match Outcome (Home Win, Away Win, or Draw).
*   **Data Engineering:** 
    *   Removal of attributes with more than 50% missing values (due to lack of historical records in early decades).
    *   Application of **One-Hot Encoding** to categorical variables (Teams and States) to prevent distance-based algorithms from erroneously inferring hierarchical order from text strings.

#### 2. Continuous Regression: Steam Games Pricing
*   **Dataset:** Steam Games Dataset (Kaggle), containing metrics and metadata for thousands of titles.
*   **Target Variable:** Game Price ($).
*   **Data Engineering:**
    *   Removal of pure text metadata and Free-to-Play games, as their monetization relies on microtransactions not captured by the features.
    *   **Feature Scaling:** Application of **Standardization** (Z-score) instead of Normalization. This was a critical mathematical decision to preserve data variance, preventing extreme outliers (viral games with millions of players) from crushing the proportional distances required by SVR and KNN models.
    *   Random sampling of 10,000 instances to ensure computational viability for complex distance algorithms during Cross-Validation.

### 🧠 Machine Learning Pipeline
For both datasets, the architecture ensures strict protection against data leakage and guarantees optimal hyperparameter selection:
*   **Architecture:** `sklearn.pipeline.Pipeline` combined with `ColumnTransformer`.
*   **Optimization:** `GridSearchCV` exploring hyperparameter grids (e.g., Hidden Layer Sizes, Activation Functions, Max Depth, Neighbors).
*   **Validation:** K-Fold Cross-Validation (CV=5).

### 🤖 Models Evaluated
The following algorithms were trained, tuned, and compared for both Classification and Regression tasks:
*   **Linear Models:** Logistic Regression (Classification) & Linear Regression (Regression).
*   **Distance-Based:** K-Nearest Neighbors (KNN Classifier & Regressor).
*   **Tree-Based:** Decision Trees (Classifier & Regressor).
*   **Neural Networks:** Multilayer Perceptron (MLP Classifier & Regressor).
*   **Vector-Based:** Support Vector Machines (SVC & SVR).

### 📈 Evaluation Metrics
The notebooks include comprehensive data visualizations (Heatmaps and Scatter Plots) and compare models using:
*   **Classification:** Accuracy, Precision, Recall, F1-Score, and Confusion Matrices.
*   **Regression:** R² (Coefficient of Determination), MAE (Mean Absolute Error), and MSE (Mean Squared Error).

### 🚀 How to Explore
1. Clone the main repository.
2. Navigate to this specific project folder.
3. Open the `.ipynb` files using Jupyter Notebook, JupyterLab, or VS Code to interact with the code, read the step-by-step mathematical reasoning, and view the generated charts natively.

---
**Developed by:** Gabriel Raulino Dal Pont

</details>

<details>
<summary>🇧🇷 <b>Ler em Português (BR)</b></summary>
<br>

Este repositório contém experimentos acadêmicos desenvolvidos para a disciplina de Inteligência Artificial na UFSC. O projeto foca na aplicação prática de algoritmos clássicos de Machine Learning utilizando `scikit-learn` para resolver dois problemas distintos do mundo real: Classificação Multiclasse e Regressão Contínua.

### 🎯 Objetivos e Datasets

#### 1. Classificação Multiclasse: Campeonato Brasileiro
*   **Dataset:** Dados históricos das partidas do Campeonato Brasileiro.
*   **Variável Alvo:** Resultado da Partida (Vitória do Mandante, Vitória do Visitante ou Empate).
*   **Engenharia de Dados:** 
    *   Remoção de atributos com mais de 50% de dados faltantes (falta de registros em décadas anteriores).
    *   Aplicação de **One-Hot Encoding** nas variáveis categóricas (Times e Estados) para evitar que algoritmos baseados em distância inferissem falsas hierarquias a partir de textos.

#### 2. Regressão Contínua: Precificação de Jogos na Steam
*   **Dataset:** Steam Games Dataset (Kaggle), contendo métricas e metadados de milhares de títulos.
*   **Variável Alvo:** Preço do Jogo ($).
*   **Engenharia de Dados:**
    *   Filtro de metadados textuais e remoção de jogos gratuitos (Free-to-Play), pois a monetização destes se baseia em microtransações não mapeadas pelas features.
    *   **Escalonamento (Feature Scaling):** Aplicação de **Padronização** (StandardScaler) em vez de Normalização. Decisão matemática crítica para preservar a variância dos dados, impedindo que *outliers* extremos (jogos virais com milhões de jogadores) destruíssem as distâncias proporcionais exigidas pelos modelos SVR e KNN.
    *   Amostragem aleatória de 10.000 instâncias para viabilizar o custo computacional de algoritmos de distância durante a Validação Cruzada.

### 🧠 Pipeline de Machine Learning
Para ambos os datasets, a arquitetura garante proteção estrita contra vazamento de dados (*data leakage*) e otimização de parâmetros:
*   **Arquitetura:** `sklearn.pipeline.Pipeline` combinado com `ColumnTransformer`.
*   **Otimização:** `GridSearchCV` explorando grades de hiperparâmetros (ex: Camadas Ocultas, Funções de Ativação, Profundidade Máxima da Árvore, K-Vizinhos).
*   **Validação:** Validação Cruzada K-Fold (CV=5).

### 🤖 Modelos Avaliados
Os seguintes algoritmos foram treinados, otimizados e comparados tanto nas tarefas de Classificação quanto de Regressão:
*   **Modelos Lineares:** Regressão Logística (Classificação) e Regressão Linear (Regressão).
*   **Baseados em Distância:** K-Nearest Neighbors (KNN Classifier & Regressor).
*   **Baseados em Árvore:** Árvore de Decisão (Classifier & Regressor).
*   **Redes Neurais:** Multilayer Perceptron (MLP Classifier & Regressor).
*   **Baseados em Vetor:** Support Vector Machines (SVC & SVR).

### 📈 Métricas de Avaliação
Os notebooks incluem visualizações de dados detalhadas (Mapas de Calor e Gráficos de Dispersão) e comparam o desempenho usando:
*   **Classificação:** Acurácia, Precision, Recall, F1-Score e Matrizes de Confusão.
*   **Regressão:** R² (Coeficiente de Determinação), MAE (Erro Absoluto Médio) e MSE (Erro Quadrático Médio).

### 🚀 Como Explorar
1. Clone o repositório principal.
2. Navegue até o diretório específico deste projeto.
3. Abra os arquivos `.ipynb` utilizando Jupyter Notebook, JupyterLab ou VS Code para interagir com o código, ler o raciocínio matemático passo a passo e visualizar os gráficos gerados nativamente.

---
**Desenvolvido por:** Gabriel Raulino Dal Pont

</details>