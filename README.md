# 🧠 Artificial Intelligence: Algorithms & Experiments

<details>
<summary>🇺🇸 <b>Read in English</b></summary>
<br>

This repository serves as a centralized portfolio of Artificial Intelligence and Machine Learning experiments. It contains practical implementations of classical and modern algorithms developed to solve complex problems, ranging from predictive data analysis to robotic control and computer vision.

### 📂 Repository Structure

Navigate through the folders below to explore the detailed documentation, mathematical reasoning, and native `.ipynb` implementations for each specific domain:

* 📊 **[Supervised Learning](./Supervised-Learning):** Multiclass Classification (Sports Analytics) and Continuous Regression (Steam Games Pricing) using linear models, distance-based algorithms, and Support Vector Machines.
* 🤖 **[Reinforcement Learning](./Reinforcement-Learning):** Optimization and motor control in discrete (`LunarLander-v2`) and continuous (`BipedalWalker-v3`) environments, comparing Q-Learning, DQN, PPO, and SAC algorithms.
* 🧬 **[Deep Learning](./Deep-Learning):** Convolutional Neural Networks (CNNs) built from scratch using PyTorch for Earth observation and Land Cover Classification (EuroSAT).

### 🚀 Getting Started

Follow these steps to run the notebooks locally.

**1. Clone the repository**
```bash
git clone https://github.com/Gabriel-Raulino/Machine-Learning-Experiments.git
cd Machine-Learning-Experiments
```

**2. Create and activate a virtual environment** *(recommended)*
```bash
python -m venv .venv

# Windows
.venv\Scripts\activate

# macOS / Linux
source .venv/bin/activate
```

**3. Install the dependencies**
```bash
pip install -r requirements.txt
```

**4. Launch Jupyter**
```bash
jupyter notebook
```
Then open any `.ipynb` file from the `Supervised-Learning`, `Reinforcement-Learning`, or `Deep-Learning` folders and run the cells from top to bottom (`Kernel → Restart & Run All` is recommended to guarantee code and outputs are in sync).

> **Note:** The Supervised Learning and Deep Learning notebooks download their datasets automatically via `kagglehub` / `torchvision`. The Reinforcement Learning notebooks require `gymnasium[box2d]` (already listed in `requirements.txt`) for the `LunarLander-v2` and `BipedalWalker-v3` environments.

---
**Developed by:** Gabriel Raulino Dal Pont

</details>

<details>
<summary>🇧🇷 <b>Ler em Português (BR)</b></summary>
<br>

Este repositório serve como um portfólio centralizado de experimentos em Inteligência Artificial e Machine Learning. Ele contém implementações práticas de algoritmos clássicos e modernos desenvolvidos para resolver problemas complexos, desde análise preditiva de dados até controle robótico e visão computacional.

### 📂 Estrutura do Repositório

Navegue pelas pastas abaixo para explorar a documentação detalhada, o raciocínio matemático e as implementações nativas em `.ipynb` para cada domínio específico:

* 📊 **[Aprendizado Supervisionado](./Supervised-Learning):** Classificação Multiclasse (Análise Esportiva) e Regressão Contínua (Precificação de Jogos) utilizando modelos lineares, baseados em distância e Support Vector Machines.
* 🤖 **[Aprendizado por Reforço](./Reinforcement-Learning):** Otimização e controle motor em ambientes discretos (`LunarLander-v2`) e contínuos (`BipedalWalker-v3`), comparando algoritmos Q-Learning, DQN, PPO e SAC.
* 🧬 **[Aprendizado Profundo](./Deep-Learning):** Redes Neurais Convolucionais (CNNs) construídas do zero com PyTorch para observação da Terra e classificação do uso do solo (EuroSAT).

### 🚀 Como Executar

Siga os passos abaixo para rodar os notebooks localmente.

**1. Clone o repositório**
```bash
git clone https://github.com/Gabriel-Raulino/Machine-Learning-Experiments.git
cd Machine-Learning-Experiments
```

**2. Crie e ative um ambiente virtual** *(recomendado)*
```bash
python -m venv .venv

# Windows
.venv\Scripts\activate

# macOS / Linux
source .venv/bin/activate
```

**3. Instale as dependências**
```bash
pip install -r requirements.txt
```

**4. Inicie o Jupyter**
```bash
jupyter notebook
```
Depois abra qualquer arquivo `.ipynb` dentro das pastas `Supervised-Learning`, `Reinforcement-Learning` ou `Deep-Learning` e execute as células de cima para baixo (recomenda-se usar `Kernel → Restart & Run All` para garantir que o código e os resultados salvos estejam sincronizados).

> **Observação:** Os notebooks de Aprendizado Supervisionado e Profundo baixam seus datasets automaticamente via `kagglehub` / `torchvision`. Os notebooks de Aprendizado por Reforço exigem `gymnasium[box2d]` (já incluído no `requirements.txt`) para os ambientes `LunarLander-v2` e `BipedalWalker-v3`.

---
**Desenvolvido por:** Gabriel Raulino Dal Pont

</details>
