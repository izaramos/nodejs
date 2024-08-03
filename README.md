# Progamação Web- Node.js

![Sistema de Agendamento de Consultas Médicas](https://github.com/izaramos/nodejs/blob/main/logoNode.png)

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

**Walmart:** No ano de 2013, a empresa migrou todo o seu tráfego mobile para o Node.js durante o período da Black Friday. Foi percebido que seus servidores chegaram a apenas 1% de utilização com 200 milhões de usuários online. `https://dejanglozic.com/2014/03/04/nodeday-2014/`

**PayPal:** Desenvolveu uma aplicação com Node.js e Java, que teve 33% menos linhas de código e 40% menos arquivos, dobrou o número de requisições por segundo e diminuiu em 35% o tempo de resposta. `https://medium.com/paypal-tech/node-js-at-paypal-4e2d1d08ce4f`

**Outras empresas que utilizam o Node.js:**
- Netflix
- LinkedIn
- New York Times
- Flickr
- Mozilla
-- Yahoo

