# desafio-migração-bth

Este documento descreve o desafio para MIgração de dados de multiplas origens para um repositório unico.

### Rotinas para Migração de dados de diversas fontes

Uma empresa fornecedora de software irá implantar sua solução para controle de acessos em um cliente, porém esse cliente adicionou em contrato uma cláusula obrigando a nova fornecedora realizar a importação dos dados existentes em sua base antiga no novo software a ser utilizado.

Os desafios observados nesse projeto são que os dados atuais do cliente estão armazenados em cada dispositivo de acesso, já a nova solução necessita que os dados sejam armazenados em um repositório único.
### Itens obrigatórios

* Os registros de pessoas deverão tornar-se únicos na base de destino; 
* Informações das pessoas devem ser mesclados no formato adição de informação oriundas das diversas fonte garantindo gerar informação o mais completo possível; 
Observação: Optar sempre pelo campo que contenha dados. 
* Sempre que houver conflito de dados das pessoas, optar pelo registro mais recente; 
* Os registros de locais de acesso deverão tornar-se únicos na base de destino; 
* Os locais onde as mesmas possuem acesso devem continuar inalterados; 
* A migração deve permitir a execução de forma automática e por qualquer outro profissional da empresa; 
* Possibilidade de executar mais de uma vez o processo na base de destino sem gerar duplicidade nos registros já existentes na base; 
* Deve carregar todos os registros de apontamento de acesso com seus devidos locais. 
* Caso existam inconformidade nos dados, essas devem ser apresentadas ao técnico que está executando o processo de carga;
* Possibilidade e reutilizar rotinas em novos cliente com a mesma estrutura

### Itens desejáveis

* Disponibilizar relatório de anomalias contendo inconsistências e advertências;
* Mecanismo para identificar mudanças da estrutura de origem;
* Documentação que descreva passo a passo como executar o processo de carga de dados;

### Requisitos não funcionais

### Instruções para entrega

* Fazer um fork desse projeto, desenvolver e enviar o link do repositório.
* Documentar todos passos para rodar as rotinas.
* O histórico do Git também será avaliado.
* Entregas parcias também serão aceitas e avaliadas.
