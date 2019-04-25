# desafio-migração-bth

Este documento descreve o desafio para migração de dados de multiplas origens para um repositório unico.

### Rotinas para Migração de dados de diversas fontes

Uma empresa fornecedora de software irá implantar sua solução para controle de acesso em um cliente, porém esse cliente adicionou em contrato uma cláusula obrigando a nova fornecedora a realizar a importação dos dados existentes em sua base antiga no novo software a ser utilizado.

Os desafios observados nesse projeto são que os dados atuais do cliente estão armazenados em cada dispositivo de acesso, já a nova solução necessita que os dados sejam armazenados em um repositório único.
### Itens obrigatórios

* Os registros de pessoas deverão tornar-se únicos na base de destino; 
* As informações das pessoas devem ser unificadas com o objetivo de garantir um registro mais completo; 
* Sempre que ocorrer conflito de dados das pessoas, optar pelo registro mais recente; 
* Os registros de locais de acesso deverão tornar-se únicos na base de destino; 
* Os locais onde as pessoas possuem acesso devem continuar inalterados; 
* O processo de migração deve permitir execução de forma automática
* O processo de migração deverá permitir a execução por qualquer outro profissional da empresa; 
* Permitir ser executado mais de uma vez o processo na base de destino sem gerar duplicidade nos registros; 
* Deve carregar todos os registros de apontamento de acesso com seus devidos locais. 
* Caso exista inconformidade nos dados, essas devem ser tratadas e apresentadas ao técnico que está executando o processo de carga;
* Possibilidade de reutilizar as rotinas de migração em novos cliente que posuam a mesma estrutura sem necessidade de alterações;

### Itens desejáveis

* Disponibilizar relatório de anomalias contendo inconsistências e advertências;
* Mecanismo para identificar mudanças da estrutura de origem;
* Documentação descrevendo passo-a-passo como executar o processo de carga de dados;

### Instruções 

* Arquivos com a estrutura de dados do sistema de destino <br/>

###[Estrutura_dados_controle_acesso.sql]: https://raw.githubusercontent.com/vanersonBorba/desafio-migracao-bth/master/Estrutura_dados_controle_acesso.sql

* Arquivos de dados 

###[ponto1.csv]: https://raw.githubusercontent.com/vanersonBorba/desafio-migracao-bth/master/ponto1.csv
[ponto2.csv]: https://raw.githubusercontent.com/vanersonBorba/desafio-migracao-bth/master/ponto2.csv
[ponto3.csv]: https://raw.githubusercontent.com/vanersonBorba/desafio-migracao-bth/master/ponto3.csv
[ponto4.csv]: https://raw.githubusercontent.com/vanersonBorba/desafio-migracao-bth/master/ponto4.csv
[ponto5.json]: https://raw.githubusercontent.com/vanersonBorba/desafio-migracao-bth/master/ponto5.json

[marcacoes1.csv]: https://raw.githubusercontent.com/vanersonBorba/desafio-migracao-bth/master/marcacoes1.csv
[marcacoes2.csv]: https://raw.githubusercontent.com/vanersonBorba/desafio-migracao-bth/master/marcacoes2.csv
[marcacoes3.csv]: https://raw.githubusercontent.com/vanersonBorba/desafio-migracao-bth/master/marcacoes3.csv
[marcacoes4.csv]: https://raw.githubusercontent.com/vanersonBorba/desafio-migracao-bth/master/marcacoes4.csv
[marcacoes5.json]: https://raw.githubusercontent.com/vanersonBorba/desafio-migracao-bth/master/marcacoes5.json


### Instruções para entrega

* Fazer um fork desse projeto, desenvolver e enviar o link do repositório.
* Documentar todos passos para rodar as rotinas.
* O histórico do Git também será avaliado.
* Entregas parcias também serão aceitas e avaliadas.
