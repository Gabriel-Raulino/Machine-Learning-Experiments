# 🤖 Reinforcement Learning: Discrete & Continuous Control

<details>
<summary>🇺🇸 <b>Read in English</b></summary>
<br>

This repository section contains practical implementations of Reinforcement Learning (RL) agents trained to solve complex control optimization problems using the `Gymnasium` (OpenAI Gym) framework. The project explores the fundamental differences between discrete and continuous observation/action spaces, comparing classical tabular methods with state-of-the-art Deep Reinforcement Learning algorithms.

### 🚀 Environments & Algorithms

#### 1. Discrete Environment: LunarLander-v2
* **Objective:** Optimize the trajectory of a lunar lander to safely touch down on a landing pad (coordinates 0,0) while minimizing fuel consumption and preventing crashes.
* **Action Space:** Discrete (4 actions: Do nothing, Fire left engine, Fire main engine, Fire right engine).
* **Observation Space:** 8-dimensional vector (Coordinates, Linear/Angular Velocities, Leg contact sensors).
* **Algorithms Evaluated:**
    * **Q-Learning (Tabular):** Implementation of the classic Bellman equation.
    * **DQN (Deep Q-Network):** Integration of Deep Learning to approximate the Q-values, effectively mapping the 8D continuous observation space to discrete actions without requiring manual state discretization.

#### 2. Continuous Environment: BipedalWalker-v3
* **Objective:** Advanced motor control problem where a bipedal robot must walk/run forward to the end of the terrain without falling, optimizing its motor energy expenditure.
* **Action Space:** Continuous (4 dimensions: Torque control for Hip 1, Knee 1, Hip 2, Knee 2 ranging from -1.0 to 1.0).
* **Algorithms Evaluated:**
    * **PPO (Proximal Policy Optimization):** An *On-Policy* algorithm used as the baseline.
    * **SAC (Soft Actor-Critic):** An *Off-Policy* algorithm utilizing Entropy Maximization.

### 🧠 Key Insights & Conclusions
The most significant finding of this project revolves around the efficiency of exploration strategies in high-dimensional continuous spaces (BipedalWalker). 

Under restricted exploration budgets, the **PPO** (On-Policy) algorithm severely penalized the agent, leading to premature convergence into local optima. In contrast, the **SAC** (Off-Policy) algorithm proved incredibly effective. By leveraging **Entropy Maximization**, SAC actively forced the robot out of its "comfort zone," encouraging robust trajectory exploration. The agent successfully learned that advancing efficiently yielded infinitely more rewards than the occasional penalty for falling, reaching the Global Optimum.

### 🛠️ Tech Stack
* `Python 3.11+`
* `Gymnasium` (Environments)
* `Stable-Baselines3` (PPO, SAC, DQN architectures)
* `PyTorch` (Backend engine for neural networks)
* `NumPy` & `Matplotlib` (Metrics and Moving Average analysis)

---
**Developed by:** Gabriel Raulino Dal Pont & Eduardo Pires

</details>

<details>
<summary>🇧🇷 <b>Ler em Português (BR)</b></summary>
<br>

Esta seção do repositório contém implementações práticas de agentes de Aprendizado por Reforço (RL) treinados para resolver problemas complexos de otimização de controle utilizando o framework `Gymnasium` (OpenAI Gym). O projeto explora as diferenças fundamentais entre espaços de ação/observação discretos e contínuos, comparando métodos clássicos tabulares com algoritmos de Deep Reinforcement Learning no estado da arte.

### 🚀 Ambientes e Algoritmos

#### 1. Ambiente Discreto: LunarLander-v2
* **Objetivo:** Otimizar a trajetória de um módulo lunar para pousar com segurança na base (coordenadas 0,0), minimizando o consumo de combustível e evitando colisões.
* **Espaço de Ação:** Discreto (4 ações: Inércia, Motor esquerdo, Motor central, Motor direito).
* **Espaço de Observação:** Vetor de 8 dimensões (Coordenadas, Velocidades Lineares/Angulares, Sensores de contato das pernas).
* **Algoritmos Avaliados:**
    * **Q-Learning (Tabular):** Implementação clássica da equação de Bellman.
    * **DQN (Deep Q-Network):** Integração de Deep Learning para aproximar os Q-values, mapeando eficientemente o espaço de observação contínuo (8D) para ações discretas, dispensando a discretização manual de estados.

#### 2. Ambiente Contínuo: BipedalWalker-v3
* **Objetivo:** Problema avançado de controle motor onde um robô bípede deve caminhar/correr até o final do terreno sem cair, otimizando o gasto de energia de suas articulações.
* **Espaço de Ação:** Contínuo (4 dimensões: Controle de torque para Quadril 1, Joelho 1, Quadril 2 e Joelho 2, variando de -1.0 a 1.0).
* **Algoritmos Avaliados:**
    * **PPO (Proximal Policy Optimization):** Algoritmo *On-Policy* utilizado como base de comparação.
    * **SAC (Soft Actor-Critic):** Algoritmo *Off-Policy* que utiliza Maximização de Entropia.

### 🧠 Principais Descobertas e Conclusões
O *insight* mais significativo deste projeto diz respeito à eficiência das estratégias de exploração em espaços contínuos de alta dimensionalidade (BipedalWalker). 

Sob orçamentos de exploração (timesteps) restritos, o algoritmo **PPO** (*On-Policy*) penalizou severamente o agente, levando-o a uma convergência prematura em ótimos locais. Em contrapartida, o algoritmo **SAC** (*Off-Policy*) mostrou-se incrivelmente eficaz. Através do conceito de **Maximização de Entropia**, o SAC forçou o robô a sair da sua zona de conforto de forma sistemática. O agente confirmou que os pontos de distância (avanço no terreno) recompensavam infinitamente mais do que as punições eventuais por quedas, alcançando convergência total para o Ótimo Global.

### 🛠️ Tecnologias Utilizadas
* `Python 3.11+`
* `Gymnasium` (Ambientes)
* `Stable-Baselines3` (Arquiteturas PPO, SAC, DQN)
* `PyTorch` (Motor matemático das Redes Neurais)
* `NumPy` & `Matplotlib` (Análise de métricas e médias móveis)

---
**Desenvolvido por:** Gabriel Raulino Dal Pont & Eduardo Pires

</details>