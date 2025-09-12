# AULA 02

[<- VOLTAR](https://github.com/igorcardiias?tab=repositories)

 <br>

 * Diferença entre **Banco De Dados Relacional** e **Banco De Dados Não Relacional**

## Diferença entre o SQL e o NOSQL

 **SQL (Structured Query Language é uma linguagem de programação padrão para gerenciar bancos de dados relacionais)** 

 <br>

 **NOSQL (Not Only SQL" Não apenas SQL e refere-se a bancos de dados não relacionais que gerenciam e armazenam dados de formas flexíveis, não baseadas em tabelas tradicionais com esquemas fixos.)**


 ## Diferença entre Monolito e Micro Serviços

 **Monolito**: um monolito refere-se a uma arquitetura de software onde todas as funcionalidades e componentes do sistema estão unificados num único código base, formando uma aplicação única e autossuficiente. Em vez de ser dividido em serviços menores e independentes, o "monolito" opera como uma única unidade, compartilhando recursos de processamento e dados, o que pode facilitar o desenvolvimento inicial, mas apresenta desafios de escalabilidade e manutenção à medida que o aplicativo cresce. 

 **Micro Serviços**: Um microsserviço é um pequeno componente de um aplicativo maior, responsável por uma função específica e que funciona de forma independente. Diferente de um sistema monolítico, onde tudo está numa única unidade, a arquitetura de microsserviços divide uma aplicação em serviços menores, flexíveis e com bases de código separadas. Estes microsserviços comunicam-se por meio de APIs e cada um pode ter sua própria tecnologia e base de dados.

## Limitações do Banco de Dados Relacionais

### Rigidez e Estrutura

**Estrutura Fixa**:
O modelo relacional exige uma estrutura de tabelas e relacionamentos pré-definida, o que pode dificultar a adaptação a alterações nos requisitos do sistema.
<br>

**Não Suporta Dados Não Estruturados**:
A estrutura baseada em tabelas não é ideal para armazenar dados não estruturados ou semiestruturados, como documentos, imagens ou vídeos. 
<br>

**Limitação de Atributos**:
Atributos multivalorados (que podem ter vários valores) são geralmente não permitidos, exigindo que cada atributo tenha um valor único e atômico. 
<br>

### Escalabilidade e Desempenho: 

**Dificuldade em Escalar Horizontalmente**:
A escalabilidade horizontal (distribuir dados em vários servidores) é mais complexa em bancos de dados relacionais comparada com outros tipos de sistemas.

**Complexidade de Consultas**:
Em grandes volumes de dados, consultas complexas podem comprometer o desempenho, pois o sistema pode precisar de mais recursos de processamento.

### Manutenção e Flexibilidade
<br>

**Manutenção Complexa**:
Com o crescimento do volume de dados, a manutenção e otimização do banco de dados relacional podem se tornar tarefas complexas e demoradas. 
<br>

**Flexibilidade Limitada**:
A necessidade de definir todas as restrições e relacionamentos de antemão pode reduzir a flexibilidade do sistema a longo prazo. 

## Limitações do Banco de Dados Não Relacionais
**Escalabilidade Vertical**: Distribuiçoes em multiplos servidores.
<br>

**Esquema Flexível**: Estrutura dinâmica e evolutivas.
<br>

**Modelos Diversos**: Documento, chave-valor, coluna, grafo
<br>

**Performance**: Otimizado para operações especificas
<br>

**BASE**: Basically avalible, Soft state, Eventually consistent

 [<- VOLTAR](https://github.com/igorcardiias/Banco-de-Dados-N-o-Relacionais.git)
