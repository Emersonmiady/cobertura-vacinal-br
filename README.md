# Cobertura Vacinal: uma análise dos dados de Sarampo no Brasil
---
Este projeto foi desenvolvido durante o **Bootcamp de Data Science Aplicada (Alura)**, no Módulo 2. Neste módulo treinamos um pouco mais a parte de **Manipulação e Visualização de Dados**, possibilitando assim melhorar as nossas analises futuras. As aulas foram feitas em cima dos dados financeiros do SUS.

Como desafio, foi requisitado uma análise da **cobertura vacinal** de alguma doença, podendo retirar informações do DATASUS ou de um outro local, e o assunto que foi escolhido por mim foi sobre o **Sarampo**.

# Contexto
---
Poderíamos resumir 2020 em uma única palavra: "pandemia". A COVID-19 foi o assunto desse ano e, infelizmente, deixou grandes números de casos e mortes. 

Entretanto, não podemos nos esquecer que, desde 2018, casos de Sarampo voltaram a aparecer, e esta doença possui uma taxa de contágio **6x** maior que o novo coronavírus. A pergunta que fica é, por que as pessoas não estão se vacinando contra o Sarampo? Será que existe diferença nas coberturas vacinais dependendo da Região ou UF no Brasil? 

Estes foram assuntos que quis trazer para meu projeto, e com uma **análise descritiva** junto de pesquisas no Google, achei algumas respostas possíveis.

**Base de dados:**
- Incidência de sarampo no Brasil, de 1980 a 2019 (WHO);
- Estimativa da cobertura vacinal mundial de sarampo, entre 2000 e 2019 (WHO);
- Cobertura vacinal brasileira, no país, nas regiões e nas UF's, entre 2000 e 2019 (TABNET - DATASUS).

# Ferramentas utilizadas
---
- Linguagem de programação Python;
- Pacotes: pandas, numpy, datetime, matplotlib, seaborn, IPython;
- Notebook: Google Colaboratory.

# Descrição breve das etapas
---
## 1. Pré-processamento
- Extração dos dados brasileiros no *DataFrame* da WHO e pesquisas para descobrir o valor faltante dos casos de sarampo no ano de 2017;
- Extração do ano de 2000 a 2019 e exclusão da linha "Total", no conjunto de dados do DATASUS (Região brasileira);
- Realizando vários "*melts*" nos dados do DATASUS (Regiões e Estados) e depois, agrupando estes em um *Dataframe* principal.

## 2. Análise Exploratória dos Dados
O que mais foi utilizado foram gráficos de linhas, por conta dos dados seguirem uma ordem temporal. Algumas visualizações abaixo:
![](https://github.com/Emersonmiady/cobertura-vacinal-br/blob/main/img/br_world.png?raw=true)
![](https://github.com/Emersonmiady/cobertura-vacinal-br/blob/main/img/measles_br.png?raw=true)
![](https://github.com/Emersonmiady/cobertura-vacinal-br/blob/main/img/br_regions.png?raw=true)

## 3. Possíveis motivos para a não vacinação
1. Horários, redução de clínicas e falta de confiança;
2. Hesitação vacinal;
3. Movimentos Anti-vacina.

