# 🦟 Tech Challenge Fase 1 - Suporte ao Diagnóstico de Chikungunya

Este repositório contém a solução desenvolvida para o **Tech Challenge da 1ª Fase** da Pós-Graduação em **IA para Devs** pelo **Grupo 9**. O projeto foca na aplicação de algoritmos de Machine Learning para otimizar a triagem de arboviroses em um ambiente de Hospital Universitário.

---

## 👥 Nosso Grupo - Grupo 9
* **Ana Paula Rodrigues Pereira** (RM 369663) - aninha-felicio@hotmail.com
* **Debora Priscila de Oliveira** (RM 370133) - deborapoh@gmail.com
* **Leander Seefeld** (RM 370115) - leanseefeld@gmail.com
* **Nurielly Caroline Brizola** (RM 370109) - nurycaroline@gmail.com
* **Rodrigo Figueiredo de Deus** (RM 370140) - rodrigo_fdedeus@hotmail.com 

---

## 🎲 Contexto e Base de Dados
O desafio proposto consiste em criar um sistema inteligente que auxilie equipes clínicas na análise inicial de prontuários e exames.

A base de dados utilizada provém do **SINAN (Sistema de Informação de Agravos de Notificação)**, contendo registros de notificações de **Chikungunya** do ano de 2025. O foco é a **Classificação Binária** entre casos Confirmados e Descartados, onde o custo de um **Falso Negativo** (não detectar a doença) é a prioridade crítica a ser minimizada.

---

## 🔄 Ciclo de Vida do Desenvolvimento (MLOps)
O projeto foi estruturado seguindo as melhores práticas de Ciência de Dados:

1.  **Análise e Limpeza (EDA):** Identificação de correlações e tratamento de colunas com alta taxa de dados faltantes (>99%).
2.  **Engenharia de Atributos:** Seleção de sintomas clínicos (Febre, Artralgia, Mialgia) e comorbidades para alimentar os modelos.
3.  **Avaliação de Estratégias:** Comparação rigorosa entre modelos de **Regressão** (Linear e Random Forest) e **Classificação**.
4.  **Modelagem:** Implementação de múltiplos algoritmos: Random Forest, KNN, XGBoost e LightGBM.
5.  **Validação Clínica:** Uso de Matrizes de Confusão e F1-Score para minimizar o risco de Falsos Negativos.

---

## 📊 Resultados e Conclusão
Após os testes, o modelo **XGBoost Classifier** foi o selecionado para a solução final, apresentando:
* **Acurácia:** 0.9689
* **F1-Score:** 0.9547
* **Justificativa:** O modelo demonstrou o melhor equilíbrio para evitar falsos negativos, sendo robusto para o processamento de grandes volumes de dados epidemiológicos.

---

## 📒 Documentação Técnica e Vídeo
* **Notebook do Projeto:** [Acesse o Notebook Principal](./tech-challenge-chikungunya.ipynb)
* **Vídeo Explicativo:** [Assista à apresentação no YouTube](https://youtu.be/8BiieKbi8uk) **#TODO: colocar o link do video**

---

### 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3.14
* **Bibliotecas Principais:** Pandas, Scikit-Learn, XGBoost, LightGBM, Seaborn e Matplotlib.
* **Abordagem:** Classificação Binária (Supervisionada).

---

## 🛠️ Como Executar
1. Clone o repositório.
2. Tenha o Python devidamente instalado (caso não esteja rodando no Google Colab.)
2. Abra o arquivo `tech-challenge-chikungunya.ipynb` em um ambiente Jupyter ou Google Colab.
4. Certifique-se de que a base de dados `CHIKBR25.csv` esteja na pasta correta indicada no notebook.

---

## 🚀 Atividade Complementar: Visão Computacional na Saúde

Além da análise preditiva baseada em dados tabulares do SINAN, o grupo desenvolveu um estudo avançado utilizando **Deep Learning** para o auxílio ao diagnóstico por imagem.

Explorando a frente de **Visão Computacional**, implementamos uma **Rede Neural Convolucional (CNN)** focada na detecção de câncer de mama. O projeto utiliza o dataset [BreaKHis (Breast Cancer Histopathological Image Dataset)](https://www.kaggle.com/datasets/ambarish/breakhis).

A arquitetura desenvolvida visa automatizar a triagem inicial de exames, identificando padrões suspeitos e auxiliando a equipe médica na priorização de casos críticos, reduzindo o tempo de resposta diagnóstica em ambientes hospitalares.

O desenvolvimento completo desta análise, incluindo a arquitetura da rede, o pré-processamento das imagens e as métricas de validação, pode ser consultado no repositório oficial do grupo:

👉 **[Acesse aqui o Notebook e a Base de dados da Atividade Extra (CNN - Breast Cancer)](https://drive.google.com/drive/folders/19jXpa3xlQ_FiFFPe7NphtAW1B6Tixoi8)