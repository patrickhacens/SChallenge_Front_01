# SENAI Frontend Challenge 01.01

Este é um desafio de desenvolvimento de software para avaliar suas habilidades relacionadas a area de frontend.

Dentro desse repositório você irá encontrar 3 releases, para windows, linux e macos, todos em 64bits.
Essas releases permitirão que você execute a API, essa API estará rodando na porta 5000 **sem HTTPS**. O seu entregável desse teste deverá se integrar com essa API.
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
Para atingir os requisitos abaixo descritos você pode adicionar quantos projetos/bibliotecas achar necessário, **porém utilizar React é um grande plus**.

É requerido ambas as **interfaces** e **integrações** das funcionalidades.

### Autenticação
> 
> Deverá haver uma tela para autenticar no sistema. Porém apenas a funcionalidade de cadastro de eventos requer autenticação então para isso você deverá criar um componente de perfil visualizado no canto superior direito da plataforma, permitindo acessar a tela de autenticação caso desautenticado e fazer logout. A autenticação é feita através de um token JWT que deverá ser enviado em todas as requisições quando autenticado no Header Authorization no formato: `Bearer {token}`.
> 
> Você também deverá persistir a autenticação sendo que quando fechar a janela a aba no browser e abrir denovo o estado de autenticação deverá se manter.
>

### Menu lateral
>
> Deverá haver um menu lateral que permita o acesso aos requisitos abaixo.
>

### Gestão de usuários

#### Listar
> 
> Deverá listar os usuários do sistema, de forma paginada.
> 

#### Criar
> 
> Deverá permitir inserir as informações para cadastrar um usuário.
> 

#### Remover
> 
> Deverá ser um componente na lista de usuários que o permita exclui-lo.
> 

### Gestão de eventos

#### Cadastrar
> 
> Deverá permitir cadastrar um usuário, o endpoint para essa ação requer autenticação e a interface também deverá trata-lo.
> 

#### Listar
> 
> Deverá permitir listar os eventos de forma paginada.
> Deverá também possuir filtros de data minima e máxima, esses filtros deverão ser opcionais.
> 

#### Detalhar
> 
> Deverá mostrar todos as informações de um evento e deve estar disponivel a partir da interface de listagem.
> 

#### Editar
> 
> Deverá permitir alterar as informações de um evento conforme o que a API disponibiliza.
> 

#### Remover
> 
> Deverá permitir remover um evento, deverá também estar disponivel através da interface de listagem e de detalhe.
> 

### Dashboard

#### Eventos Anuais
> 
> Deverá mostrar os dados dos eventos anuais com um filtro de ano que deverá iniciar no ano atual.
> 

#### Eventos por usuário
> 
> Deverá mostrar os dados de eventos por usuário.
>

#### Top 10 eventos com mais participantes
>
> Deverá mostrar um ranking com os top 10 eventos com mais participantes
>

### Execução
> 
> Você deverá adicionar no README.md os passos necessários para builder e executar o seu projeto se necessário
> 

## Entrega
Você deverá criar um pull request com suas alterações para esse repositório.
**É necessário apontar o e-mail usado no processo seletivo dentro do arquivo README.md**.
Qualquer outras informação que você queira compartilhar sobre como alguma requisito funciona ou algo que seja necessário você pode descrever no seu README.md
