# Sistema de Controle de Oficina Mecânica

## Objetivo
Este projeto visa o desenvolvimento de um sistema de controle e gerenciamento de ordens de serviço para uma oficina mecânica, incluindo a gestão de clientes, veículos, mecânicos, serviços e peças.

## Narrativa
O sistema deve gerenciar o processo de execução de ordens de serviço em uma oficina mecânica. Os clientes levam seus veículos para consertos ou revisões periódicas. Cada veículo é associado a uma ordem de serviço (OS), que inclui a data de emissão, os serviços a serem executados, os valores das peças e serviços, e a data de conclusão.

## Entidades
- **Cliente**: informações sobre os clientes que levam os veículos à oficina.
- **Veículo**: informações sobre os veículos que serão consertados ou revisados.
- **Mecânico**: dados sobre os mecânicos da oficina, como especialidade e nome.
- **Ordem de Serviço (OS)**: informações sobre a ordem de serviço, incluindo número, data de emissão, valor, status e data de conclusão.
- **Serviço**: tipos de serviços executados, com valores de mão-de-obra.
- **Peça**: informações sobre as peças necessárias para o conserto.
- **Tabela de Mão-de-Obra**: valores por hora para os diferentes tipos de serviços executados.

## Relacionamentos
- **Cliente-possui-Veículo**: Um cliente pode ter vários veículos.
- **Veículo-recebe-OS**: Cada veículo recebe uma ordem de serviço.
- **OS-contém-Serviço**: A OS pode conter múltiplos serviços a serem executados.
- **OS-usa-Peça**: A OS pode envolver várias peças.
- **Equipe-executa-OS**: Equipes de mecânicos executam as ordens de serviço.
- **Mecânico-participa-Equipe**: Mecânicos fazem parte de equipes responsáveis pelas OSs.
- **Tabela de Mão-de-Obra-calcula-Serviço**: A tabela de mão-de-obra determina os custos dos serviços executados.

## Solução Adotada
O modelo conceitual proposto foi implementado através de um diagrama de Entidade-Relacionamento (ER) que relaciona as entidades, atributos e os respectivos relacionamentos entre elas, utilizando a ferramenta MySQL Workbench para gerar o modelo e os scripts necessários para implementação do banco de dados.

## Instruções
- O diagrama de ER está disponível no arquivo `diagrama-oficina.mwb`.
- O banco de dados pode ser implementado utilizando os scripts SQL gerados pela ferramenta MySQL Workbench.
