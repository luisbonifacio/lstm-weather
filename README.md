# LSTM para prever Temperaturas de Dry Bulb
## Introdução

A temperatura de Dry Bulb, normalmente chamada de "temperatura do ar", é a propriedade do ar mais comumente utilizada.[1]

É chamada de "Dry Bulb" porque a temperatura do ar é indicada por um termômetro que não é afetado pela Umidade do ar. [1]

A temperatura de Dew Point é a temperatura em que o vampor de água começa a condensar no ar (a temperatura na qual o ar se torna completamente saturado).  Acima dessa temperatura, o orvalho começa a se formar.[1]

 - Se a temperatura de Dew-Point está próxima da temperatura do ar (Dry bulb temperature) - A umidade relativa é alta.
 - Se a temperatura de Dew-Point muito abaixo da temperatura do ar - A umidade relativa é baixa.

 
Quando a temperatura do Dry Bulb é reduzida ao Dew-Point, começam a se formar: nevoeiro, orvalho, geada, nuvens, chuva, granizo ou neve.[2]

Na aviação, a temperatura do Dry Bulb, juntamente com a temperatura do Dew-Point, permitem saber onde está a base da nuvem, pois a nuvem se forma justamente quando elas se equiparam.[2]

## Objetivo

Dado um dataset com vários informações relativas a vôos, organizados de forma sequencial no tempo (time series), a proposta desse notebook é prever um destes atributos considerados relevantes para a tomada de decisão do piloto (aumentar ou diminuir a altitude de vôo, por exemplo).

Tendo em vista a importância do conhecimento sobre a formação e posição de nuvens por parte dor pilotos, este notebook propõe uma arquitetura de Rede neural Recorrente utilizando Células LSTM para prever a temperatura do Dry Bulb, popularmente conhecida como temperatura do ar.

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
