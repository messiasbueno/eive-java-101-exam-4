# eive-java-exam-4

## Docker / Postgres

  - Faça o clone do projeto `https://github.com/spring-projects/spring-petclinic.git`.
  - Crie o `dockerfile` necessário para a construção e execução do projeto, considere que o projeto utilizará o `spring.profiles.active` de postgres.
  - Configure o projeto para que a pasta `target` seja ignorada pelo docker ao construir a imagem.
  - Construa o projeto utilizando a seguinte tag: `eive-java-exam-4:prod`.
  - Suba a imagem para o docker hub e vincule a URL da imagem na atividade.
  - Vincule o comando necessário para rodar o container da imagem criada considerando que ela será baixada do docker hub e conectará no postgres.
    - Atenção: as credenciais de acesso ao banco devem ser informadas através de variáveis de ambiente.

  ```
  - Imagem está no dockerhub messiasdb1/eive-java-exam-4
  - Foi criado a Tag prod
  - Criado arquivo comandos.md com informações para baixar e rodar a imagem
  ```
  [comandos](./comandos.md)

## MongoDB

  - Faça o clone do respositório `https://github.com/mcampo2/mongodb-sample-databases.git`.
  - Importe o `dataset` localizado em `sample_airbnb` (mongoimport - MongoDB Database Tools).
  - Realize as seguintes operações (utilizar `mongosh` e vincular as _queries_ executadas):
    - Inserir um novo registro de imóvel para aluguel conforme estrutura já existente.
    - Alterar o valor do preço diário (`price`) para `500` do registro incluído.
    - Informar apenas o valor do apartamento com diária (`price`)  mais cara disponível no Brasil (`BR`) sem retornar o campo `_id`.
