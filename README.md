# P1_ML

Aprendizado Supervisionado

O nosso modelo aprendeu os padrões olhando para o histórico de vendas do ano passado. Ou seja, ele treinou usando dados onde a resposta certa já era conhecida.

Neste caso, nós usamos os Meses (nossa variável independente, que fica no eixo X) para tentar adivinhar as Vendas (nosso alvo, no eixo Y). 

--

Análise de Tendência

A análise indica uma clara tendência de crescimento para todos os produtos da loja.

Essa conclusão é confirmada por dois fatores principais: a inclinação da reta é maior que "0" e observamos que o volume de vendas projetado aumenta progressivamente de um trimestre para o outro.

--

Planilha de Previsão de Vendas

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
