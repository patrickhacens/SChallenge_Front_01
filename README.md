# SENAI Frontend Challenge 01.01

Este é um desafio de desenvolvimento de software para avaliar suas habilidades relacionadas a area de frontend.

Dentro desse repositório você irá encontrar 3 releases, para windows, linux e macos, todos em 64bits.
Essas releases permitirão que você execute a API que deverá se integrar com, essa API estará rodando na porta 5000 sem HTTPS.
Uma documentação SWAGGER está disponivel em http://localhost:5000/swagger/index.html você poderá usa-la para testar e auxilia-lo na integração.
O dados são persistidos enquanto a aplicação estiver rodando e possuirá dados iniciais aleatórios a cada inicialização, porém o usuário abaixo sempre estará cadastrado para facilitar os testes

> Usuario: string
> 
> Password: string

Para executar no windows abra um terminal e utilize o comando:
> SChallengeAPI.exe

Para executar no linux ou macos abra um terminal e utilize o comando:
> chmod a+x SChallengeAPI
>
> ./SChallengeAPI

Para esse desafio você deverá ***forkar*** esse repositório e altera-lo para habilitar os requisitos abaixo descritos.

## Avaliação
Será avaliado o funcionamento dos requisitos, código, design patterns e arquitetura, então não só o requisito funcional será avaliado como também toda a infraestrutura de código e algoritmos para atingir o funcionamento do requisito, por isso é recomendado que considere esse desafio, mesmo que pequeno, como um projeto de alta complexidade e mostre suas capacidades como desenvolvedor.

## Requisitos
Para atingir os requisitos abaixo descritos você pode adicionar quantos projetos/bibliotecas achar necessário. 

É requerido ambas as **interfaces** e **integrações** das funcionalidades.

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

### Execução
> 
> Você deverá adicionar no README.md os passos necessários para builder e executar o seu projeto se necessário
> 

## Entrega
Você deverá criar um pull request com suas alterações para esse repositório.
**É necessário apontar o e-mail usado no processo seletivo dentro do arquivo README.md**.
Qualquer outras informação que você queira compartilhar sobre como alguma requisito funciona ou algo que seja necessário você pode descrever no seu README.md
