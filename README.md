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

![log_idades](https://user-images.githubusercontent.com/88217999/163505936-6730b7aa-8fcb-41a0-b14a-c78b97aeefeb.png)

No gráfico de dispersão envolvendo as idades e salários há alguma indicação de que o turnover é mais frequente nas pessoas mais velhas e com maiores salários.

![idades_salarios](https://user-images.githubusercontent.com/88217999/163892032-f7275cca-2df0-4f7e-ae3e-5bbe54e543ea.png)

## Machine Learning

Foram testados diferentes modelos e o método de validação utilizado foi o K-fold.O melhor modelo foi selecionado de acordo o f1-score.Dos modelos testados, o modelo com melhor perfomance foi o Gradient Boosting.

![tabela](https://user-images.githubusercontent.com/88217999/163892995-57a86b39-e8ce-4d8d-99e2-5a02a6c0da1c.png)

As variáveis: Raça/Cor, Deficiência e UF têm pequena influência no f1-score e foram retiradas da análise.

A tunagem de hiperparâmetros não apresentou melhora no desempenho do modelo e a classificação final foi dada pelo modelo padrão de Gradient Boosting.
