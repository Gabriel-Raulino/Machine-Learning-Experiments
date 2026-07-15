# 🧬 Deep Learning: Satellite Image Classification (CNN)

<details>
<summary>🇺🇸 <b>Read in English</b></summary>
<br>

This repository section contains a Deep Learning project focused on Computer Vision, developed for the Artificial Intelligence course at UFSC. The objective is to automatically classify land use and land cover using remote sensing data, deploying Convolutional Neural Networks (CNNs) built from scratch using PyTorch.

### 🌍 The Dataset: EuroSAT
* **Source:** Sentinel-2 Satellite imagery.
* **Volume:** 27,000 expertly labeled images.
* **Format:** $64 \times 64$ pixels, RGB (3 channels).
* **Classes (10):** Annual Crop, Forest, Herbaceous Vegetation, Highway, Industrial, Pasture, Permanent Crop, Residential, River, Sea/Lake.

### 🧠 Architecture & Methodology
The core of this project is a custom **Convolutional Neural Network (CNN)**. The architecture leverages:
* **Convolutional Layers:** Applying mathematical filters (kernels) to extract spatial hierarchies and visual features (edges, textures, shapes).
* **Pooling Layers:** Dimensionality reduction to ensure spatial invariance and computational efficiency.
* **Fully Connected (Dense) Layers:** Final classification head mapping the extracted features to the 10 distinct land cover classes.

### 🔬 Experimental Tuning & Ablation Study
Following rigorous scientific methodology, the project includes an ablation study to analyze how different hyperparameter configurations impact the model's convergence and accuracy. Experiments included variations in:
* Model Depth (Number of Convolutional Layers / Filters)
* Learning Rate scheduling
* Batch Size dimensions
* Regularization techniques (e.g., Dropout) to mitigate overfitting.

### 🛠️ Tech Stack
* `Python 3.11+`
* `PyTorch` (Core Deep Learning Engine)
* `Torchvision` (Dataset loading and image transformations)
* `NumPy` & `Matplotlib` (Tensor manipulation and loss/accuracy visualization)

---
**Developed by:** Gabriel Raulino Dal Pont

</details>

<details>
<summary>🇧🇷 <b>Ler em Português (BR)</b></summary>
<br>

Esta seção do repositório contém um projeto de Aprendizado Profundo (Deep Learning) focado em Visão Computacional, desenvolvido para a disciplina de Inteligência Artificial da UFSC. O objetivo é classificar automaticamente o uso e a cobertura do solo a partir de dados de sensoriamento remoto, utilizando Redes Neurais Convolucionais (CNNs) construídas do zero com PyTorch.

### 🌍 O Dataset: EuroSAT
* **Origem:** Imagens do satélite Sentinel-2.
* **Volume:** 27.000 imagens perfeitamente rotuladas.
* **Formato:** $64 \times 64$ pixels, RGB (3 canais).
* **Classes (10):** Culturas anuais, Floresta, Vegetação Herbácea, Autoestrada, Área Industrial, Pastagem, Culturas Permanentes, Área Residencial, Rios e Mares/Lagos.

### 🧠 Arquitetura e Metodologia
O núcleo deste projeto é uma **Rede Neural Convolucional (CNN)** customizada. A arquitetura utiliza:
* **Camadas Convolucionais:** Aplicação de filtros matemáticos (*kernels*) para extrair hierarquias espaciais e características visuais (bordas, texturas, formas).
* **Camadas de Pooling:** Redução de dimensionalidade para garantir invariância espacial e eficiência computacional.
* **Camadas Totalmente Conectadas (Dense):** Classificador final que mapeia os tensores de características para as 10 classes de cobertura do solo.

### 🔬 Otimização e Estudo de Ablação
Seguindo um rigoroso método científico, o projeto inclui testes comparativos para analisar como diferentes configurações de hiperparâmetros afetam a convergência e a acurácia do modelo. Os experimentos envolveram variações em:
* Profundidade da rede (Número de camadas e filtros convolucionais)
* Taxa de Aprendizado (*Learning Rate*)
* Tamanho do Lote (*Batch Size*)
* Técnicas de Regularização (ex: *Dropout*) para mitigar o sobreajuste (*overfitting*).

### 🛠️ Tecnologias Utilizadas
* `Python 3.11+`
* `PyTorch` (Motor principal de Deep Learning)
* `Torchvision` (Carregamento do dataset e transformações de tensores)
* `NumPy` & `Matplotlib` (Manipulação de arrays e visualização de perda/acurácia)

---
**Desenvolvido por:** Gabriel Raulino Dal Pont

</details>