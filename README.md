# Previsão de Taxas de Câmbio no Mercado FOREX com Machine Learning

Este repositório contém o código e os experimentos desenvolvidos como parte do Trabalho de Conclusão de Curso (TCC) para o MBA em Data Science e Analytics. O objetivo principal é avaliar o desempenho de diferentes algoritmos de machine learning na previsão da taxa de câmbio EUR/USD no mercado FOREX, utilizando dados históricos obtidos por meio de APIs públicas.

## 📈 Objetivo

Investigar a eficácia de modelos supervisionados de aprendizado de máquina na previsão de séries temporais cambiais, com foco no par EUR/USD, aplicando:

- Regressão Linear
- Árvore de Decisão
- Random Forest
- Gradient Boosting
- Rede Neural Artificial (ANN)
- LSTM (Long Short-Term Memory)

## 🧪 Experimentos

Cada modelo foi treinado com dados históricos entre 2019 e 2024, e testado com dados reais de janeiro de 2025. O pipeline incluiu:

1. Extração de dados com `pandas_datareader` (Fonte: FRED)
2. Pré-processamento (criação de variáveis defasadas, normalização, divisão treino/teste)
3. Treinamento e avaliação com métricas:
   - RMSE (Root Mean Square Error)
   - R² (Coeficiente de Determinação)
4. Visualização dos resultados com `matplotlib`

## 📊 Resultados

Os modelos foram comparados com base no desempenho preditivo em dados reais de 2025:

| Modelo              | RMSE    | R²       |
|---------------------|---------|----------|
| Regressão Linear    | 0.00549 | 0.55130  |
| Árvores de Decisão  | 0.00990 | -0.45576 |
| Random Forest       | 0.00810 | 0.02418  |
| Gradient Boosting   | 0.00603 | 0.45959  |
| ANN (MLPRegressor)  | 0.00569 | 0.51918  |
| LSTM (Keras)        | 0.00633 | 0.29669  |

Os resultados indicam que, embora modelos complexos como LSTM e ensembles tenham bom desempenho em cenários históricos, a Regressão Linear se mostrou mais estável em dados recentes.

## 🛠️ Requisitos

- Python 3.10+
- Bibliotecas:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `scikit-learn`
  - `tensorflow` (para LSTM)
  - `pandas_datareader`

Instale os requisitos com:

```bash
pip install -r requirements.txt


MBA em Data Science e Analytics - 2025
