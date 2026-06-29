# Comparação de Técnicas de Redução de Dimensionalidade em Dados de Grande Escala

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Optuna](https://img.shields.io/badge/Optuna-Bayesian_Optimization-blue)](https://optuna.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-Machine_Learning-orange)](https://scikit-learn.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Repositório oficial com o código-fonte e os experimentos realizados para escrita do artigo **Comparação de Técnicas de Redução de Dimensionalidade em Dados de Grande Escala**, desenvolvido na Universidade Estadual Paulista "Júlio de Mesquita Filho" (UNESP). 

## 📖 Sobre o Projeto

O estudo apresenta uma análise experimental empírica sobre o impacto de diferentes técnicas de redução de dimensionalidade no pré-processamento de dados (*denoising*). Utilizando o conjunto de dados **Fashion-MNIST** corrompido com ruído sintético Gaussiano, o experimento inova ao contrastar a otimização de hiperparâmetros guiada por duas métricas distintas:
* **MSE (Erro Quadrático Médio)**: Otimização baseada no erro matemático absoluto.
* **SSIM (Índice de Similaridade Estrutural)**: Otimização focada na preservação da percepção visual, topologia e bordas das imagens.

## ⚙️ Técnicas e Algoritmos Avaliados

* **PCA** (Análise de Componentes Principais)
* **SVD** (Decomposição em Valores Singulares)
* **Kernel PCA** (com aplicação do *Kernel Trick* polinomial)

O diferencial deste projeto reside no uso do *framework* **Optuna** para a otimização Bayesiana dinâmica dos hiperparâmetros (número de componentes, tipo de kernel, coeficientes, etc.) para cada uma das métricas alvo, garantindo a extração do potencial máximo de cada modelo.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python
* **Machine Learning:** Scikit-Learn
* **Otimização de Hiperparâmetros:** Optuna
* **Processamento de Imagens e Métricas:** Scikit-Image (SSIM, PSNR, MSE)
* **Manipulação de Dados e Visualização:** NumPy, Pandas, Matplotlib
* **Ambiente de Execução:** Google Colaboratory
