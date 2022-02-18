
# <p align="center"> Projeto Módulo 04 - Grupo 08 

## <p align="center"> Data Analytics - Turma 12 - Resilia
  


## **Sobre o projeto**

Este projeto é uma análise exploratória relacionada à série histórica de preço de venda da gasolina e do etanol no Brasil. 
Ele foi desenvolvido como trabalho de final do módulo 4 do curso de Data Analytics da Resilia Educação.  

A fonte de dados utilizada foi o Portal Brasileiro de Dados Abertos, da Base de Dados da Agência Nacional do Petróleo, Gás Natural e Biocombustíveis - ANP referente a série história de junho e julho de 2021 contendo a série histórica dos preços da gasolina e do etanol em todo o Brasil.

## **Tecnologias e ferramentas utilizadas**
  
  ![python](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)
  ![markdowm](https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=white)
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VQKz_G_0E1aWVDdx6PJsTLT10oMhsRE6)
    
  * Python
  * Google Colab 


## **Nossa Equipe**

[Bruno Mendes](https://github.com/Brunoka02)

[Carla Lanzillotta](https://github.com/CarlaLanzillotta)

[Fernanda Oliveira](https://github.com/FernandaBz)  

[Reinaldo](https://github.com/reinaldos)

  
## Contextualização 
  
### **O que é ANP**

A Agência Nacional do Petróleo, Biocombustíveis e Gás Natural criada em 1997 é responsável pelas regras e resoluções de exploração, produção, refino, comercialização e transporte do petróleo e seus derivados no Brasil. Além do petróleo, a ANP regula também as atividades das indústrias de gás natural e biocombustíveis.
A agência é a responsável pela emissão de registros para postos de combustíveis e realiza semanalmente uma pesquisa nacional de preços dos combustíveis, com o objetivo de orientar os consumidores.
A ANP mantém o Banco de Dados de Exploração e Produção (BDEP), onde são publicados dados sobre a indústrias do petróleo, biocombustível e gás natural.


![anp](https://github.com/Brunoka02/Projeto_4/blob/main/Anp-logo-3menor.png)

### **Objetivo da análise**
Esta análise tem como objetivo observar a variação de preços de venda de combustíveis reltivos ao período de junho e julho de 2021 para compreender melhor se dados como localidade e tranporte podem interferir nos valores finais de venda dos produtos. Além de ajudar a elaborar meios para diminuição de custos de transporte. Esses dados estão disponíveis no Portal Brasileiro de Dados Abertos - https://dados.gov.br/anp.

## **Conhecendo os dados**
Na etapa seguinte partimos para a importação das bibliotecas e em uma análise de que tipo de dados tínhamos para lidar.

![import10](https://github.com/Brunoka02/Projeto_4/blob/main/10.png)

Cálculo do percentual de dados faltantes dos datasets
```
(junho_21.isnull().sum() / junho_21.shape[0]).sort_values(ascending=False)
```

Conhecemos também os tipos de dados contidos nos datasets
```
display(junho_21.dtypes)
```

## **Análise Exploratória e limpeza/correção de dados**  
Foram concatenados os dois datasets para que fosse possível unificar os valores referentes aos dois meses apresentados. 
Em seguida realizada a análise exploratória e limpeza de dados.  
    
![import12](https://github.com/Brunoka02/Projeto_4/blob/main/12.png)

Além da correção do valor dos indices após a concatenação  
  
![import1](https://github.com/Brunoka02/Projeto_4/blob/main/13.png)
 
Conversão de tipos do dataset

![import1](https://github.com/Brunoka02/Projeto_4/blob/main/18.png)

![import1](https://github.com/Brunoka02/Projeto_4/blob/main/19.png)
  
## **Análise dos dados a partir das questões solicitadas**
Nesta etapa enfim fizemos a análise dos dados a partir das questões seguintes e de mais duas adicionadas pela equipe.
  
* Como se comportaram o preço dos combustíveis durante os dois meses
citados? Os valores do etanol e da gasolina tiveram uma tendência de
queda ou diminuição?
* Qual o preço médio da gasolina e do etanol nesses dois meses?
* Quais os 5 estados com o preço médio da gasolina e do etanol mais
caros?
* Qual o preço médio da gasolina e do etanol por estado?
* Qual o município que possui o menor preço para a gasolina e para o
etanol?
* Qual o município que possui o maior preço para a gasolina e para o
etanol?
* Qual a região que possui o maior valor médio da gasolina?
* Qual a região que possui o menor valor médio do etanol?
* Há alguma correlação entre o valor do combustível (gasolina e etanol) e a
região onde ele é vendido?
* Há alguma correlação entre o valor do combustível (gasolina e etanol) e a
bandeira que vende ele?

A análise completa pode ser encontrada também no [notebook](https://colab.research.google.com/drive/1VQKz_G_0E1aWVDdx6PJsTLT10oMhsRE6#scrollTo=XtYjHHVm_Cha) rodando todas as células em sequência.
  
