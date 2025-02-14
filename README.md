# 🏥**Predição de Câncer utilizando Machine Learning e Bioinformática**

![Badge](https://img.shields.io/badge/Machine%20Learning-Random%20Forest-blue)
![Badge](https://img.shields.io/badge/Bioinformática-Genômica-green)

## 🔍**Introdução**
Este projeto utiliza **Machine Learning** para a predição de câncer com base em dados genéticos e históricos clínicos dos pacientes. Foi desenvolvido um modelo Random Forest para realizar a classificação, garantindo alta precisão na detecção da doença.

---

 ## 📌**Objetivo do Projeto**
 
 ✅ Aplicar técnicas de pré - processamento, com o intuito de deixar os dados prontos para o desenvolvimento e implementação do modelo.
 
 ✅ Realizar análise exploratória dos dados para identificar padrões nos dados e correlações entre as features presentes no conjuntos de dados.
 
 ✅ Construir um modelo de Random Forest para predição do câncer.
 
 ✅ Avaliar o desempenho do modelo e interpretar os resultados.
 
 ---
 
 ## 🛠️**Tecnologias Utilizadas**
🔹Linguagem: Python

🔹`Bibliotecas Principais:`
 * Pandas e NumPy (Manipulação de dados)
 * Matplotlib e Seaborn (Visualizações)
 * Scikit - Learn (Machine Learning)
 * Imbalancead - learn (Balanceamento de classes - SMOTE)
 
---

## 📂**Estrutura do Projeto**
|- README.MD (Epílogo Projeto)

|- Base de Dados Pacientes (Conjuntos de dados utilizado para o desenvolvimento)

|- Predição Cancêr.ipynb (Notebook que obtém as analises e o modelo criado)

---

## 💡**Principais Descobertas**

* 1️⃣ *Historico_Familiar e Diagnostico_Cancer:*

Indivíduos com histórico familiar de câncer tem uma chance ligeiramente maior de serem diagnosticados com a doença. Certamente, isso acontece porque temos uma correlação positiva moderada entre essas duas variáveis que foi identificado pelo gráfico de mapa de calor.

* 2️⃣ *Gene3_Expressao, Gene4_Expressao e Diagnostico_Cancer*
  
Isso indica que pacientes que possuem níveis altes de expressão do Gene 3 e 4 podem ter uma maior probabilidade serem diagnosticados com câncer.

* 3️⃣ *Sexo e Diagnostico_Cancer*
  
Encontramos uma correlação entre o gêneros dos pacientes e o diagnostico de câncer, mas este protocole está muito mais associado aos aspectos femininos do que masculinos. Portanto, é importante salientar que por ela ser uma correlação negativa ela se torna "fraca", e isso significa que a relação não é determinante e que temos outros fatores que desempenham papéis mais importantes para o desenvolvimento da doença.

---

## 🧰**Desenvolvimento do Modelo e Avaliação**

Foi desenvolvido um modelo de classificação `Random Forest`, com o objetivo de termos uma generalização eficiente e um baixo indice de overfitting.

Desta forma, abaixo temos as configurações que foram feitas para o treinamento do modelo:

***Configurações do Modelo***

🔹Importação da biblioteca SMOTE para aplicar a técnica over-sampling (Aumentar valores na classe minoritaria) realizando assim um balanceamento na base de treino.

🔹Uso do parâmetro class_weight="balanced" para minimizar o impacto do desbalanceamento das classes.

🔹Definição de random_state = 42 para garantir reprodutibilidade (Capacidade de obter os mesmos resultados a partir dos mesmos dados e códigos por diferentes ambientes).

***Avaliação do Modelo***

✅ O modelo atingiu 100% de acurácia, precisão, recall e F1-Score, demonstrando um desempenho excepecional.

✅ Nenhuma amostra foi classificada incorretamente, indicando que o modelo está altamente eficaz na distinção entre casos positivos e negativos.

✅ A aplicação da técnica over-sampling e do ajuste de pesos foi essencial para equilibrar os dados e garantir a alta performace do modelo.

✅ A análise de importância das variáveis revelou que a expressão genética dos genes 3 e 4 são os principais indicadores para o diagnóstico.

