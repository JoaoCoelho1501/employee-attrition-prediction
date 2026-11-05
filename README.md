# Previsão de Saída de Colaboradores (Employee Attrition)

> Classificação binária com dados de uma competição Kaggle: EDA, pipelines de pré-processamento, desequilíbrio de classes, comparação de modelos e análise de equidade (fairness).

**Mestrado em Business Intelligence & Analytics (ISCAP)**, 2025/26

## O problema
Prever que colaboradores têm maior probabilidade de sair da empresa, para que os RH possam agir a tempo.

## Abordagem
1. **EDA**: distribuições, relação com o target, correlações e *data drift* entre treino e teste.
2. **Pré-processamento**: feature engineering, pipelines do scikit-learn e tratamento do desequilíbrio de classes.
3. **Modelação**: Logistic Regression como baseline, Random Forest, Gradient Boosting, redes neuronais e KNN, avaliados com validação cruzada estratificada.
4. **Fairness**: comparação do risco previsto e dos erros por grupos, como género e faixa etária.

## Resultado
O **Gradient Boosting** foi o modelo final: teve o ROC-AUC mais alto, bom recall na classe minoritária e desempenho estável entre folds. As variáveis mais associadas à saída são remuneração, antiguidade, horas extra e função.

> O modelo deve **apoiar** a decisão dos RH e não substituí-la, com monitorização periódica da equidade.

## Stack
`pandas` · `scikit-learn` · `matplotlib`

Dados: [Kaggle Playground Series S3E3](https://www.kaggle.com/competitions/playground-series-s3e3)

## Autores
Beatriz Teixeira · João Coelho
