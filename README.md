<h1>**Pequeno projeto para um desafio avançado da DIO**</h1>

<h4>Este consite em mostrar meus filmes favoritos que estão na AWS DynamoDB através da AWS CLI</h4>

<h5>Segue comando utilizados</h5>

<h5>**Criar uma tabela:**</h5>

aws dynamodb create-table --cli-input-json file://FavoriteMovies.json --region us-east-2

<h5>**Inserir um item na tabela:**</h5>

aws dynamodb put-item --table-name FavoriteMovies --item file://itemmovies.json --region us-east-2

<h5>**Inserir vários itens na tabela:**</h5>

aws dynamodb batch-write-item --request-items file://batchmovies.json --region us-east-2
