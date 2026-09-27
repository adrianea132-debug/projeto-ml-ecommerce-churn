# Projeto ML - E-commerce Churn

Pipeline preditivo de Machine Learning para prever quais clientes de um e-commerce estão prestes a cancelar (churn), permitindo que a empresa aja preventivamente com ações de retenção.

## 📊 Sobre o Projeto

Este projeto foi desenvolvido como parte da disciplina de Machine Learning e Visão Computacional. O objetivo é identificar clientes com alta probabilidade de churn, para que a empresa possa oferecer incentivos (como cupons) antes que eles cancelem.

## 🗂️ Dataset

Base de dados de e-commerce com 5.630 clientes e 20 variáveis, incluindo tempo de casa (Tenure), forma de pagamento preferida, satisfação, uso de cupons, entre outras.

## 🔧 Etapas do Projeto

1. **Análise Exploratória de Dados (EDA):** identificação de desbalanceamento na variável alvo (~17% churn) e padrões nas variáveis.
2. **Limpeza de Dados:** tratamento de nulos com mediana e outliers com capping (Z-Score).
3. **Feature Engineering:** criação da coluna `cashback_por_pedido`.
4. **Separação, Balanceamento e Escalonamento:** encoding, split estratificado, SMOTE (apenas no treino) e StandardScaler.
5. **Modelagem:** comparação entre KNN (K=3,5,7,9) e Árvore de Decisão (profundidades 3,5,7,ilimitada), com análise de overfitting.
6. **Avaliação:** matriz de confusão e recomendação final de modelo para produção.

## 🏆 Resultado Final

Modelo recomendado: **KNN (K=7)**

Apesar de menor acurácia geral, o KNN apresentou recall superior para a classe de churn, minimizando o erro mais custoso para o negócio: deixar de identificar um cliente que realmente vai cancelar.

## 🛠️ Tecnologias Utilizadas

- Python (Google Colab)
- Pandas, NumPy
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Matplotlib, Seaborn

## 🎥 Vídeo de Apresentação

[Link do vídeo aqui]

## 👤 Autora

Adriane Araujo
