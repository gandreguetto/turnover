# Turnover após 1 ano
## O conjunto de dados e objetivo

Esse conjunto de dados apresenta dados de funcionários de diferentes empresas e indica se o funcionário deixou a empresa após 1 ano ou não (turnover após 1 ano). O conjunto apresenta 11 colunas, sendo uma contendo a resposta sobre o turnover e as outras 10 apresentam diversas características sobre os funcionários e as empresas onde trabalham. 

Temos as seguintes variáveis:

* Categóricas
    * Sexo
    * Raça/Cor
    * Escolaridade
    * UF
    * Deficiência
    * Porte da empresa
    * Setor da empresa
    * Turnover

* Numéricas
    * Idade
    * Horas de trabalho
    * Salário
    
O objetivo dessa análise é empregar modelos de classificação e investigar a capacidade desses de prever o turnover.

## Análise exploratória

Há uma diferença significativa no turnover entre homens e mulheres. Uma fração maior das mulheres deixa um emprego após 1 ano.

![sexo](https://user-images.githubusercontent.com/88217999/163504807-29db0024-df7c-425d-a4f2-89ae07eeb4e5.png)

A distribuição das idades é assimétrica à direita.

![idades](https://user-images.githubusercontent.com/88217999/163505612-2489acac-3e8d-48b8-ba16-fbaf435551f1.png)

Nós aplicamos uma transformação logarítmica nas idades o obtemos uma distribuição mais próxima da normal.


