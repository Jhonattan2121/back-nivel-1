

# back-nivel-1
 
O que é Node.js?

JavaScript no back-end
Nao lidamos ccom eventos do usuario final
rotas e integrações

plataforma(nao linguagem)

o node é contruida em cima da v8

comparavel a PHP Ruby Python Go

/////////////////////////////////////////////////////////////////

O que é NPM?

instalar bibliotecas de terceiros

fornecer bibliotecas 

por que utilizar o yarn do que o NPM?
é mais rapido 

NPM é comparavel a

composer do PHP
gems do Ruby
PIP do Python

////////////////////////////////////////////////////////////////////

Caracteristicas do node

arquitetura Event-Loop

baseada em eventos (rotas na maioria das vezes)

call Stack

ELe é em single-tread

C++ por tras com libuv

background threads

Non-blocking I/O input e output nao bloqueante 

///////////////////////////////////////////////////////////////////////

entenda como callStack funciona

é uma pilha 

uma funçao vai pra dentro da callstack

event loop vai monitorando utilizando o single-tread


////////////////////////////////////////////////////////

primeiro projeto codigos

yarn init -y 

codigos no terminal 

yarn add express/ ele cria rotas

returno de rota "response" 

retorna dados seguindo com json 

///////////////////////////////////////////////////////////////

atualização automatica 
yarn add nodemon -D 

executar nodemon 
yarn nodemon src/index.js

disparada automatica quando for subir o servidor 
app.listen(3333, () => {
    console.log('back-end started')
})

 ////////////////////////////////////////////////////////


as rotas utilizam metodos HTTP

GET http://minhaapi.com/users
    quando a gente quer buscar uma informação

POST http://minhaapi.com/users
    quer criar uma informação

PUT http://minhaapi.com/users/1
    alterar alguma informação

Delete http://minhaapi.com/users/1
deletar alguma informação

(Users) recurso/Rota
(GET, POST, PUT, DELETE) metodos HTTP
(Criar um novo usuario) Parametro


HTTP  codes

todo HTTP que inica com 1XX é informatiional
todo HTTP que inica com 2XX é SUccess
    200 SUccess
    201 created
3xx redirrection
    301 moved permanently
    302 moved
4xx  client error
    400 bad request
    401 unauthorized
    404 not found
5xx server error
    500 intterrnal server error

