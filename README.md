# P1_ML

Aqui rolou uma análise de **Aprendizado Supervisionado**. 

Mas o que isso significa? Basicamente, o nosso modelo (a famosa Regressão Linear Simples) aprendeu os padrões olhando para o histórico de vendas do ano passado. Ou seja, ele treinou usando dados onde a "resposta certa" já era conhecida (o que a gente chama na área de *dados rotulados*). É como estudar para a prova já tendo o gabarito do lado!

Neste caso, nós usamos os Meses (nossa variável independente ou *feature*, que fica no eixo X) para tentar adivinhar as Vendas (nosso alvo ou *target*, no eixo Y). 

E tem um detalhe importante: como estamos tentando prever valores numéricos contínuos de vendas (como 150, 200 ou 300 unidades) em vez de separar as coisas em categorias (tipo "vendeu muito" ou "vendeu pouco"), a gente classifica esse projeto especificamente como um problema de **Regressão**.




## Análise de Tendência

A análise indica uma clara tendência de **crescimento** para todos os produtos da loja.

Essa conclusão é confirmada por dois fatores principais:
1. **Matemática (Inclinação Positiva):** Em todos os modelos gerados, o valor de `a` (inclinação da reta) é maior que zero. Isso comprova matematicamente que as vendas sobem a cada mês que passa.
2. **Evolução Trimestral:** Ao agrupar as previsões, observamos que o volume de vendas projetado aumenta progressivamente de um trimestre para o outro. O Trimestre 5 (meses 13, 14 e 15) apresenta a maior estimativa de vendas de todo o período analisado.


# Projeto de Machine Learning: Previsão de Vendas de Tintas

## Tipo de Análise
Esta é uma análise de **Aprendizado Supervisionado**. Isso ocorre porque o modelo (Regressão Linear Simples) aprende a partir de um histórico de dados onde a "resposta correta" já é conhecida (*dados rotulados*). Neste caso, utilizamos a variável independente ou *feature* (Mês - eixo X) para prever um alvo ou *target* contínuo (Vendas - eixo Y). Como estamos prevendo valores numéricos contínuos em vez de categorias, trata-se especificamente de um problema de **Regressão**.


## Parâmetros da Regressão e Confiabilidade
Aplicamos a Equação da Reta ($y = ax + b$) para cada produto. Abaixo estão a inclinação ($a$), o coeficiente linear ($b$) e o Coeficiente de Determinação ($R^2$), que mede a taxa de acerto/confiabilidade do modelo:

1. **Tinta Acrílica:** - $a$ (inclinação): 19.09 
   - $b$ (coef. linear): 89.24 
   - **$R^2$:** 0.7985 (Aprox. 80% de confiabilidade)
2. **Tinta Esmalte:** - $a$ (inclinação): 10.87 
   - $b$ (coef. linear): 71.82 
   - **$R^2$:** 0.9817 (Aprox. 98% de confiabilidade)
3. **Tinta Látex:** - $a$ (inclinação): 10.00 
   - $b$ (coef. linear): 190.00 
   - **$R^2$:** 1.0000 (100% de confiabilidade matemática na amostra)
4. **Tinta Spray:** - $a$ (inclinação): 5.98 
   - $b$ (coef. linear): 53.64 
   - **$R^2$:** 0.9784 (Aprox. 98% de confiabilidade)
5. **Tinta PVA:** - $a$ (inclinação): 10.00 
   - $b$ (coef. linear): 140.00 
   - **$R^2$:** 1.0000 *(Nota: O R² é 1 porque há apenas 2 meses de dados históricos, gerando uma reta perfeita).*

##  Previsão para os Próximos 3 Meses (Mês 13, 14 e 15)

Utilizando os modelos gerados, prevemos o seguinte volume de vendas (em unidades):

| Produto | Mês 13 | Mês 14 | Mês 15 |
| :--- | :--- | :--- | :--- |
| **Tinta Acrílica** | 337 | 357 | 376 |
| **Tinta Esmalte** | 213 | 224 | 235 |
| **Tinta Látex** | 320 | 330 | 340 |
| **Tinta Spray** | 131 | 137 | 143 |
| **Tinta PVA** | 270 | 280 | 290 |


##  Previsão Agrupada por Trimestre e Tendência

Agrupando a soma das vendas previstas (históricas e futuras) de cada produto por trimestre:

* **T1 (Meses 1-3):** Acrílica (382), Esmalte (281), Látex (630), Spray (197), PVA (780 - *considerando a projeção para o mês 3*)
* **T2 (Meses 4-6):** Acrílica (554), Esmalte (379), Látex (720), Spray (251)
* **T3 (Meses 7-9):** Acrílica (726), Esmalte (476), Látex (810), Spray (304)
* **T4 (Meses 10-12):** Acrílica (898), Esmalte (574), Látex (900), Spray (358)
* **T5 (Meses 13-15 - Futuro):** Acrílica (1070), Esmalte (672), Látex (990), Spray (412), PVA (840)

**Análise da Tendência:**
A tendência indica um **crescimento constante** para todos os produtos. O coeficiente de inclinação ($a$) é positivo para todas as tintas. Analisando a soma trimestral, o volume de vendas projetado sobe consistentemente de um trimestre para o outro. Se o comportamento de mercado se mantiver de acordo com o ano anterior, espera-se que os três próximos meses batam os recordes de vendas de seus respectivos produtos.


### 📊 Planilha de Previsão de Vendas

| Produto | Mês | Vendas reais | Vendas previstas (ŷ) | R² |
| :--- | :---: | :---: | :---: | :---: |
| Tinta Acrílica | 1 | 120 | 108.33 | 0.7985 |
| Tinta Acrílica | 2 | 150 | 127.42 | 0.7985 |
| Tinta Acrílica | 3 | 130 | 146.52 | 0.7985 |
| Tinta Acrílica | 4 | 180 | 165.61 | 0.7985 |
| Tinta Acrílica | 5 | 200 | 184.70 | 0.7985 |
| Tinta Acrílica | 6 | 210 | 203.79 | 0.7985 |
| Tinta Acrílica | 7 | 190 | 222.88 | 0.7985 |
| Tinta Acrílica | 8 | 220 | 241.97 | 0.7985 |
| Tinta Acrílica | 9 | 210 | 261.06 | 0.7985 |
| Tinta Acrílica | 10 | 250 | 280.15 | 0.7985 |
| Tinta Acrílica | 11 | 300 | 299.24 | 0.7985 |
| Tinta Acrílica | 12 | 400 | 318.33 | 0.7985 |
| **Tinta Acrílica** | **13** | **-** | **337.42** | **0.7985** |
| **Tinta Acrílica** | **14** | **-** | **356.52** | **0.7985** |
| **Tinta Acrílica** | **15** | **-** | **375.61** | **0.7985** |
| Tinta Esmalte | 1 | 80 | 82.69 | 0.9817 |
| Tinta Esmalte | 2 | 100 | 93.57 | 0.9817 |
| Tinta Esmalte | 3 | 90 | 104.44 | 0.9817 |
| Tinta Esmalte | 4 | 120 | 115.31 | 0.9817 |
| Tinta Esmalte | 5 | 130 | 126.19 | 0.9817 |
| Tinta Esmalte | 6 | 140 | 137.06 | 0.9817 |
| Tinta Esmalte | 7 | 150 | 147.94 | 0.9817 |
| Tinta Esmalte | 8 | 160 | 158.81 | 0.9817 |
| Tinta Esmalte | 9 | 170 | 169.69 | 0.9817 |
| Tinta Esmalte | 10 | 180 | 180.56 | 0.9817 |
| Tinta Esmalte | 11 | 190 | 191.43 | 0.9817 |
| Tinta Esmalte | 12 | 200 | 202.31 | 0.9817 |
| **Tinta Esmalte** | **13** | **-** | **213.18** | **0.9817** |
| **Tinta Esmalte** | **14** | **-** | **224.06** | **0.9817** |
| **Tinta Esmalte** | **15** | **-** | **234.93** | **0.9817** |
| Tinta Látex | 1 | 200 | 200.00 | 1.0000 |
| Tinta Látex | 2 | 210 | 210.00 | 1.0000 |
| Tinta Látex | 3 | 220 | 220.00 | 1.0000 |
| Tinta Látex | 4 | 230 | 230.00 | 1.0000 |
| Tinta Látex | 5 | 240 | 240.00 | 1.0000 |
| Tinta Látex | 6 | 250 | 250.00 | 1.0000 |
| Tinta Látex | 7 | 260 | 260.00 | 1.0000 |
| Tinta Látex | 8 | 270 | 270.00 | 1.0000 |
| Tinta Látex | 9 | 280 | 280.00 | 1.0000 |
| Tinta Látex | 10 | 290 | 290.00 | 1.0000 |
| Tinta Látex | 11 | 300 | 300.00 | 1.0000 |
| Tinta Látex | 12 | 310 | 310.00 | 1.0000 |
| **Tinta Látex** | **13** | **-** | **320.00** | **1.0000** |
| **Tinta Látex** | **14** | **-** | **330.00** | **1.0000** |
| **Tinta Látex** | **15** | **-** | **340.00** | **1.0000** |
| Tinta Spray | 1 | 60 | 59.62 | 0.9784 |
| Tinta Spray | 2 | 70 | 65.59 | 0.9784 |
| Tinta Spray | 3 | 65 | 71.57 | 0.9784 |
| Tinta Spray | 4 | 80 | 77.55 | 0.9784 |
| Tinta Spray | 5 | 85 | 83.53 | 0.9784 |
| Tinta Spray | 6 | 90 | 89.51 | 0.9784 |
| Tinta Spray | 7 | 95 | 95.49 | 0.9784 |
| Tinta Spray | 8 | 100 | 101.47 | 0.9784 |
| Tinta Spray | 9 | 105 | 107.45 | 0.9784 |
| Tinta Spray | 10 | 110 | 113.43 | 0.9784 |
| Tinta Spray | 11 | 120 | 119.41 | 0.9784 |
| Tinta Spray | 12 | 130 | 125.38 | 0.9784 |
| **Tinta Spray** | **13** | **-** | **131.36** | **0.9784** |
| **Tinta Spray** | **14** | **-** | **137.34** | **0.9784** |
| **Tinta Spray** | **15** | **-** | **143.32** | **0.9784** |
| Tinta PVA | 1 | 150 | 150.00 | 1.0000 |
| Tinta PVA | 2 | 160 | 160.00 | 1.0000 |
| **Tinta PVA** | **13** | **-** | **270.00** | **1.0000** |
| **Tinta PVA** | **14** | **-** | **280.00** | **1.0000** |
| **Tinta PVA** | **15** | **-** | **290.00** | **1.0000** |





