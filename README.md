# Classificação de Crédito

Este projeto tem como objetivo desenvolver um modelo preditivo para identificar o risco de inadimplência em uma base de proponentes de cartão de crédito. A inadimplência é definida tipicamente pela ocorrência de um atraso maior ou igual a 90 dias em um horizonte de 12 meses.

## Atividades do CRISP-DM:

### Objetivos do Negócio
O objetivo principal deste projeto é construir um modelo que sirva ao mutuário (o cliente) para auxiliá-lo na avaliação de suas próprias decisões de crédito, não visando diretamente a instituição de crédito.

### Objetivos da Modelagem
Desenvolver o melhor modelo preditivo possível para auxiliar o mutuário em suas decisões de crédito.

### Contextualização
Nesta etapa, avaliamos a situação da empresa/segmento, entendendo o tamanho do público, relevância, problemas presentes e detalhes do processo gerador do fenômeno (inadimplência). Isso inclui uma análise da base de dados disponível.

### Seleção da Técnica de Modelagem
Utilizaremos a técnica de floresta aleatória (random forest), uma abordagem versátil e robusta para capturar padrões complexos nos dados. Esta técnica é escolhida por sua eficácia em problemas de classificação como o de inadimplência.

### Desenho do Teste
Antes de executar o modelo, dividimos a base em treinamento e teste. Isso permite avaliar o desempenho do algoritmo de forma mais fidedigna.

### Avaliação do Modelo
A avaliação será feita através da acurácia do modelo, comparando as classificações previstas com o estado real de inadimplência. A acurácia é uma métrica comum de avaliação, representando a porcentagem de acertos do modelo.

## Avaliação Financeira
A avaliação financeira considera o impacto do modelo no negócio. Por exemplo, se um cliente bom pagador deixa em média 5 'dinheiros' de lucro e um mau pagador deixa em média 100 'dinheiros' de prejuízo, a matriz de confusão pode ser utilizada para calcular o impacto financeiro real.

Decisão | Lucro dos Bons | Lucro dos Maus | Total
--- | --- | --- | ---
Aprovar | 4042 x 5 | 72 x (-100) | 13,010
Reprovar | 27 x 5 | 22 x (-100) | -2,065

Neste exemplo, o modelo evitaria um prejuízo de -2,145 'dinheiros', indicando um potencial aumento no lucro através da utilização do modelo.

Este README oferece uma visão geral do projeto de classificação de crédito, abordando desde os objetivos até a avaliação financeira, destacando a importância do modelo na tomada de decisões do mutuário.
