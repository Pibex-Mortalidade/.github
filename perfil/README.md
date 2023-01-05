## Pibex-Mortalidade
 
<div align="center"><b>Repositório relativo as análise estatísticas desenvolvidas ao longo do projeto.</b></div>

### Informações Básicas
> <div align="justify">Dados de diversas naturezas são divulgados cotidianamente, no entanto, ainda que o volume de dados seja cada vez maior, observa-se limitada capacidade técnica para a sua exploração e análise. No caso específico de estatísticas vitais, a pandemia veio evidenciar a necessidade da contribuição da academia na análise e visualização desses dados, no sentido de subsidiar políticas públicas essenciais na área da saúde da população. O projeto de extensão universitária será realizado junto à Diretoria de Vigilância Epidemiológica (DIVEP) da Secretaria de Saúde do Distrito Federal responsável pela coleta e disseminação de dados sobre nascimento e óbitos ocorridos no Distrito Federal. Tem como objetivo contribuir no fortalecimento da capacidade de análise e visualização de dados sobre a mortalidade no Distrito Federal, com detalhamento geográfico e características sociodemográficas.</div>

### Tabela de Conteúdo:
  1. [Informações Básicas](#informações-básicas)
  1. [Conexão ao repositório](#conexão-ao-repositório)
  1. [Boas práticas](#boas-práticas)
  1. [Scripts:](#scripts)
      1. [Importação do banco de dados SIM e SINASC](#importação-do-banco-de-dados-sim-e-sinasc)
      1. [Leitura e Analise SIM e SINASC](#leitura-e-analise-sim-e-sinasc)
  4. [Pesquisadores Responsáveis](#pesquisadores-responsáveis)

### Conexão ao repositório:

Para executar as analises propostas você precisará:
<div style="display: inline_block"><br>
  <img align="center" alt="Gabriel-R" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/rstudio/rstudio-plain.svg"(https://rstudio.com/products/rstudio/download/#download)>
</div>
Em seguida, clone o repositório de interesse por meio do comando:

```sh
git clone https://github.com/Pibex-Mortalidade/
```

<div align="center"> 
  <b>Pronto! Agora você tem acesso a todos os scripts desenvolvidos. Abaixo <b>DEVE</b> ser apresentado a ordem cronologica destes juntamente com informações a respeito do que cada script propõe-se a realizar e quando necessário sinalize os passos faltantes entre paranteses:</b> </div>

### Boas práticas

Quando for desenvolver seu código tenha em mente o caráter de <b>Reprodutibilidade</b>;
Informe os pacotes necessários para manipulação desta forma:
```R
if (!require(pacman)) {
  install.packages("pacman")
  library(pacman)
}
pacman::p_load(tidyverse, plotly, shiny)
```
Direcione os locais de arquivos sem definir seu diretório de trabalho:

```R
read_xlsx(".\\DADOS DE APOIO\\UFS.xlsx")
```
### Scripts:
#### Importação do banco de dados SIM e SINASC
> Dowload_DN.R

Inicialmente é necessário abrir o script (#Dowload_DN.R) o qual tem como finalidade baixar em seu diretório local os arquivos em formato .dbf contidos no <b>DATASUS</b>, estes por sua vez, possui informações de estatisticas vitais como o número de obitos e nascimentos nas Unidades de Federação. 

#### Leitura e Analise SIM e SINASC
> Leitura_DO.R
> Leitura_DN.R

Os scripts acima são capazes de importar e analisar os arquivos SIM e SINASC, respectivamnete.


### Pesquisadores Responsáveis

* [Ana Maria Nogales Vasconcelos (EST/UnB)](https://github.com/)
* [Gabriel José dos Reis Carvalho (EST/UnB)](https://github.com/ventania10)
* [Valeria Maria Rodrigues Fechine (EST/UnB)](https://github.com/)




