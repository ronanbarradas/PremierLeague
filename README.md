# Documentação do Projeto

## Coleta de Dados

A coleta de dados foi realizada a partir do site Transfermarket.com, especialista em estatísticas e números sobre futebol. Utilizamos APIs públicas e bancos de dados open-source. Os passos específicos da coleta foram:

1. **Identificação das Fontes de Dados**:
    - **APIs Públicas**: Utilizamos dados do Transfermarket. com para ter os dados necessários: valor dos elencos e suas pontuações nas respectivas edições da Premier League.

2. **Extração dos Dados**:
    - **CSV**: O dataset foi baixado diretamente do Transfermarket e importado para o ambiente de análise.

3. **Pré-processamento dos Dados**:
    - Atualização dos dados, adicionando estatísticas faltantes de 2018 até 2023

4. **Armazenamento dos Dados**:
    - Os dados coletados foram armazenados em um banco de dados CSV para facilitar consultas e manipulações subsequentes.

## Modelagem

A modelagem dos dados envolveu a escolha de algoritmos de machine learning apropriados e a realização de experimentos para otimizar o desempenho dos modelos. O processo foi o seguinte:

1. **Escolha dos Modelos**:
    - Para previsão de pontos conquistados, foi utilizado um modelo de **Regressão Linear**.

2. **Divisão dos Dados**:
    - Os dados foram divididos em conjuntos de treino e teste na proporção de 75/25.

3. **Avaliação dos Modelos**:
    - **Regressão Linear**: O desempenho foi avaliado utilizando o erro médio absoluto (MAE).

## Conclusões

Com base nos resultados dos nossos modelos, chegamos às seguintes conclusões:

1. **Previsão de Pontos**:
    - Dividimos o resultado do coeficiente por 10 para uma melhor compreensão do resultado. Podemos dizer que a cada 10% abaixo do time mais caro, haveria uma perda de 5.3 pontos em média. Erro Absoluto Médio foi é de 7.6, uma margem de erro aceitável num mundo de dados fartos mas de surpresas imprevisíveis como é o futebol.

2. **Recomendações**:
    - Para melhorar ainda mais a análise de valores, recomendamos um estudo também aprofundado em equipes que formam jogadores, assim diminuindo seus gastos na aquisição de estrelas.
    - Para a previsão de pontos, sugere-se a incorporação de mais variáveis como folha salarial e orçamento disponível e usado para gastos estruturais.
