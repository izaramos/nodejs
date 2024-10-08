# Progamação Web - Node.js

![Node.js](https://github.com/izaramos/nodejs/blob/main/logoNode.png)

## O que é o Node.js?

O Node é um ambiente para executar JavaScript em um servidor, sem a necessidade de utilizar um navegador. Ele possui uma arquitetura orientada a eventos, onde, utilizando loops de eventos, a ferramenta interpreta as requisições de maneira assíncrona, minimizando bloqueios. Por isso, o Node é indicado para sistemas que lidam com um número elevado de requisições.

A ideia inicial era que o Node fosse apenas um servidor, mas, após várias evoluções, tornou-se possível criar aplicações desktop (com o Node-WebKit), ambientes voltados ao desenvolvimento front-end, e montar servidores HTTP, HTTPS, DNS, TCP, entre outros.

## Sua história

- **Ano de 2009:**
  - Nascimento do Node.js.
  - Criação da primeira versão do npm (Node Package Manager).

- **Ano de 2010:**
  - Desenvolvimento do framework Express (voltado ao desenvolvimento web no Node).
  - Lançamento do Socket.io (framework criado para facilitar a implantação de Sockets).

- **Ano de 2011:**
  - O npm ganha sua versão 1.0.
  - LinkedIn e Uber adotam o Node em seus sistemas.

- **Ano de 2013:**
  - Ghost (primeira grande plataforma de blogs) passa a utilizar o Node.
  - Nascimento da ferramenta web Koa, voltada para o Node.

- **Ano de 2014:**
  - O io.js se torna o maior fork do Node, com o objetivo de introduzir o suporte ao ES6 no mercado.

- **Ano de 2015:**
  - A Node.js Foundation é inaugurada e a quarta versão da ferramenta é lançada.
  - O io.js é incorporado ao Node.

- **Ano de 2017:**
  - O Node ganha sua oitava versão.
  - A V8 introduz o Node.js em sua suíte de testes, tornando a ferramenta oficialmente um mecanismo do JavaScript.

- **Ano de 2020:**
  - O Node.js em sua versão 18 é lançado, incluindo um módulo de test runner nativo, fetch global, melhorias no V8 e novos métodos para arrays.

## Por que utilizar essa ferramenta?

Sem a utilização do Node, a forma de lidar com a concorrência das várias requisições que um sistema recebe seria criando múltiplas threads. Porém, dentro de cada thread criada, há um tempo de resposta que não é aproveitado para nada enquanto a resposta não retorna; como consequência, a CPU fica bloqueada para realizar outras operações.

Com a utilização do Node, diversas requisições podem ser executadas simultaneamente. Em vez de esperar uma resposta para a requisição, ele processa a requisição seguinte da fila. Assim que a resposta da primeira requisição chega, a ferramenta dispara um evento e o callback da requisição (ou seja, a função que executa a resposta) é colocado na fila de requisições e é executado assim que sua vez chegar, finalizando a primeira requisição.

Ele é indicado para uso em:
- APIs
- Aplicações web de chat ou colaborativas para vários usuários
- Jogos multiplayer
- Aplicações que precisam de alta escalabilidade
- Streamings

## Grandes corporações que aderiram ao uso do Node

**Walmart:** No ano de 2013, a empresa migrou todo o seu tráfego mobile para o Node.js durante o período da Black Friday. Foi percebido que seus servidores chegaram a apenas 1% de utilização com 200 milhões de usuários online. [NodeDay](https://dejanglozic.com/2014/03/04/nodeday-2014/)

**PayPal:** Desenvolveu uma aplicação com Node.js e Java, que teve 33% menos linhas de código e 40% menos arquivos, dobrou o número de requisições por segundo e diminuiu em 35% o tempo de resposta. [Medium Paypal](https://medium.com/paypal-tech/node-js-at-paypal-4e2d1d08ce4f)

**Outras empresas que utilizam o Node.js:**
- Netflix
- LinkedIn
- New York Times
- Flickr
- Mozilla
- Yahoo

## Guia de instalação do Node.js

Para instalar o node, acesse o site oficial do framework [Node.js](https://nodejs.org/pt) e instalar com o item “Descarregue o node.js”:

![siteNode](https://github.com/izaramos/nodejs/blob/main/siteNode.png)

Após o download, basta clicar no arquivo baixado e seguir os passos informados para concluir a instalação.

![instalacao_1](https://github.com/izaramos/nodejs/blob/main/instalacao_1.png)

![instalacao_2](https://github.com/izaramos/nodejs/blob/main/instalacao_2.png)

![instalacao_3](https://github.com/izaramos/nodejs/blob/main/instalacao_3.png)

![instalacao_4](https://github.com/izaramos/nodejs/blob/main/instalacao_4.png)

![instalacao_5](https://github.com/izaramos/nodejs/blob/main/instalacao_5.png)

![instalacao_6](https://github.com/izaramos/nodejs/blob/main/instalacao_6.png)

![instalacao_7](https://github.com/izaramos/nodejs/blob/main/instalacao_7.png)

Após finalizar a instalação, acesse o seu terminal e confirme que o processo foi bem sucedido por meio de:
   ```bash
   node --version
   ```

![node_version](https://github.com/izaramos/nodejs/blob/main/node_version.png)

## Guia de utilização do Node.js

Para utilizar o node, é necessário ter o JavaScript instalado, para isso basta acessar o site oficial da linguagem e fazer o seu download. ([Java](https://www.java.com/pt-BR/download/ie_manual.jsp?locale=pt_BR))

Um arquivo com extensão “.js” deve ser criado, neste tutorial ele será nomeado como “servidor.js” e requisitar a variável http.

![criaServidor](https://github.com/izaramos/nodejs/blob/main/criaServidor.png)

Essa requisição é necessária para que o node carregue o seu módulo http, responsável por criar o servidor.

Em seguida, o servidor é oficialmente criado:

![servidor](https://github.com/izaramos/nodejs/blob/main/servidor.png)

A variável “res”, é responsável por informar a resposta que será retornada para o usuário.
Utilizando ela, a função “writeHead” define no header que a requisição feita teve status 200, ou seja, foi bem sucedida e uma mensagem de sucesso é apresentada para o usuário.

Após encerrar o server, uma função “listen” é declarada e tem como objetivo receber as requisições retornadas pela porta 9000 e chamar um callback, retornando assim, uma mensagem interna.

Esses são os passos para se criar um servidor utilizando o node.js.

Para executá-lo, acesse, via terminal, a pasta onde seu arquivo foi salvo e execute:
   ```bash
   node servidor.js
   ```

Ao acessar via navegador a URL informada (`http://localhost:9000/`), a mensagem definida no código deve ser apresentada.

## Links importantes
- Site do Node.js - [nodejs.org](https://nodejs.org/pt)
- Documentação do Node.js - [nodejs.org/api](https://nodejs.org/api/)
- NodeSchool - [nodeschool.io](https://nodeschool.io/pt-br/)
- Documentação do Java - [java.com.br](https://www.java.com/pt-BR/download/ie_manual.jsp?locale=pt_BR)

## Equipe

- **Izabelle Ramos Tomé**
- **Lucas Carvalho**