# Previsão de Valor de Aluguel com Regressão Linear

Modelo de machine learning que prevê o valor do aluguel de um imóvel a partir de suas características (tamanho, número de quartos, idade, garagem e localização). Feito em Python com Pandas, Matplotlib e scikit-learn, seguindo um pipeline completo de análise.

## Etapas do projeto

1. **Análise exploratória:** distribuição das variáveis, identificação de outliers e correlações.
2. **Preparação dos dados:** verificação de valores ausentes e codificação das variáveis categóricas (localização).
3. **Construção do modelo:** regressão linear relacionando as características do imóvel ao valor do aluguel.
4. **Avaliação do modelo:** métricas de performance (R², MAE, MSE, RMSE) e análise dos resíduos.
5. **Interpretação dos resultados:** análise dos coeficientes para entender a importância de cada variável.

## Resultados

- O modelo alcançou **R² de cerca de 0,99**, com erro médio (MAE) de aproximadamente R$ 38.
- Variáveis com maior impacto no aluguel: número de quartos (cerca de +R$ 100 por quarto) e garagem (cerca de +R$ 148), além do tamanho (cerca de +R$ 10 por m²).
- A idade do imóvel tem efeito negativo: quanto mais velho, um pouco mais barato.
- Os resíduos distribuídos aleatoriamente em torno de zero indicam que a regressão linear é adequada para o conjunto de dados.

## Tecnologias

- Python 3
- Pandas
- NumPy
- Matplotlib
- scikit-learn
- Jupyter Notebook

## Como rodar

1. Instale as dependências:

```bash
pip install pandas numpy matplotlib scikit-learn notebook
```

2. Abra o notebook `previsao_aluguel.ipynb` (no Jupyter ou VSCode) e execute todas as células.

O arquivo `dataset_aluguel.csv` precisa estar na mesma pasta do notebook.
