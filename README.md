# SENAI Backend Challenge 01.01

Este é um desafio de desenvolvimento de software para avaliar suas habilidades relacionadas a area de backend.

Dentro desse repositório você irá encontrar um projeto web `SChallenge.csproj` recem criado através da DOTNET CLI usando o comando abaixo.

> dotnet new web

Para esse desafio você deverá ***forkar*** esse repositório e altera-lo para habilitar os requisitos abaixo descritos.

## Avaliação
Será avaliado o funcionamento dos requisitos, código, design patterns e arquitetura, então não só o requisito funcional será avaliado como também toda a infraestrutura de código e algoritmos para atingir o funcionamento do requisito, por isso é recomendado que considere esse desafio, mesmo que pequeno, como um projeto de alta complexidade e mostre suas capacidades como desenvolvedor.

## Requisitos
Para atingir os requisitos abaixo descritos você pode adicionar quantos projetos/bibliotecas achar necessário. 

É requerido apenas os **endpoints** das funcionalidades então não é necessário se preocupar com interfaces visuais.

Sua aplicação deverá atender o protocolo HTTP/S

### Autenticação
> 
> Deverá retornar um token que permita a autenticação e autorização do portador desse token.
> No seu repositório você deverá descrever como a sua aplicação espera que esse token seja enviado.
> 

### Gestão de usuários

#### Listar
> 
> Deverá retornar uma lista com os dados não sensiveis dos usuários cadastrados.
> 

#### Criar
> 
> Deverá receber as informações de um usuário e cadastra-lo, sendo disponibilizado no endpoint de listagem.
> 

#### Remover
> 
> Deverá receber o identificador do usuário e remove-lo, impossibilitando a listagem e autenticação dele.
> 

### Gestão de eventos
#### Dados
> Os eventos deverão possuir os seguintes dados:
>- Identificador
>- Nome do evento
>- Número de participantes
>- Data de acontecimento
>- Duração do evento
>- Criador

#### Cadastrar
> 
> Deverá receber os dados do evento, exceto criador, e cadastra-lo, a informação do criador do evento deverá pega automaticamente através do usuário autenticado e esse endpoint só poderá ser acessado por usuário autenticados.
> 

#### Listar
> 
> Deverá receber a quantidade de itens e página usados para a paginação
> e data minima e máxima (opcionais) usados como filtro através do queryparams  
> e retornar alem da lista (simplificada) paginada informações sobre a quantidade total de itens.
> 

#### Detalhar
> 
> Deverá receber o identificador do evento e trazer os dados completo desse evento.
> 

#### Editar
> 
> Deverá receber o identificador do evento a ser alterado e os novos dados do evento no payload da requisição.
> 

#### Remover
> 
> Deverá receber o identificador do evento e remove-lo.
> 

### Dashboard

#### Eventos Anuais
> 
> Deverá receber o ano e retornar por mês a quantidade de eventos que aconteceram naquele ano.
> 

#### Eventos por usuário
> 
> Deverá retornar uma lista com o usuário e a quantidade de eventos que eles criaram.
>

#### Top 10 eventos com mais participantes
>
> Deverá retornar uma lista com os 10 eventos com mais participantes ordernados do maior para o menor
>

### Swagger
> 
> Deverá haver um endpoint de documentação swagger ou openapi equivalente, você deverá documentar no seu README.md como acessa-la.
> 

### Seeding
> 
> Deverá haver uma forma, seja endpoint ou script para que o haja uma injeção inicial de dados para testes da API, documente como utilizar essa forma de seeding no seu README.md.
> 

## Entrega
Você deverá criar um pull request com suas alterações para esse repositório.
**É necessário apontar o e-mail usado no processo seletivo dentro do arquivo README.md**.
Qualquer outras informação que você queira compartilhar sobre como alguma requisito funciona ou algo que seja necessário você pode descrever no seu README.md
