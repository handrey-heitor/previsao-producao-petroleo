# Análise e Previsão da Produção de Petróleo no Campo Canto do Amaro

Este projeto apresenta uma análise de séries temporais aplicada à produção de petróleo do campo Canto do Amaro, utilizando dados mensais entre 2005 e 2022.

Os dados são inicialmente filtrados e agrupados por período com o pacote `dplyr`. Em seguida, a produção é convertida em uma série temporal mensal para análise de tendência, sazonalidade e autocorrelação.

Durante o processo de modelagem, são aplicadas a transformação de Box-Cox e a diferenciação da série, buscando estabilizar a variância e obter uma série aproximadamente estacionária. As funções ACF e PACF são utilizadas para investigar a dependência temporal e auxiliar na definição das ordens dos modelos.

A série é dividida em conjuntos de treinamento e validação. Diferentes modelos são ajustados e comparados, incluindo modelos ARIMA selecionados pelo `auto.arima`, modelos ARIMA definidos manualmente e o modelo TBATS.

O desempenho das previsões é avaliado por meio de medidas como MAE, RMSE e MAPE, além da comparação gráfica entre os valores observados e previstos. O objetivo é identificar o modelo mais adequado para representar o comportamento da série e prever a produção futura de petróleo.
