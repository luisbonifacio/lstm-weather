# LSTM para prever Temperaturas de Dry Bulb

## Objetivo

Dado um dataset com vários informações relativas a vôos, organizados de forma sequencial no tempo (time series), a proposta desse notebook é prever um destes atributos considerados relevantes para a tomada de decisão do piloto (aumentar ou diminuir a altitude de vôo, por exemplo).

Tendo em vista a importância do conhecimento sobre a formação e posição de nuvens por parte dos pilotos, este notebook propõe uma arquitetura de Rede neural Recorrente utilizando Células LSTM para prever a temperatura do Dry Bulb, popularmente conhecida como temperatura do ar.

## Sumário

1. Importações
2. Aquisição, Limpeza e Tratamento do Dataset
3. Preparação dos dados de Treino e Teste
4. Modelo RNN
5. Treinamento
6. Resultados: Previsão em Relação ao Dataset de Teste
7. Avaliação do Modelo
8. Previsão dos próximos valores
9. Referências

## Data

Os dados usados neste Notebook foram extraídos do repositório abaixo: 
The data used in this Notebook were extracted from the repository below:
https://github.com/mouradmourafiq/tensorflow-lstm-regression
