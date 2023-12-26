# Problema 2 - Mensageiro 
## Resumo
Este repositório contém os códigos fonte e recursos relacionados ao projeto de Chat em Rede Local. O projeto consiste em um sistema de chat distribuído em uma rede local, onde os usuários podem trocar mensagens em tempo real. Os códigos estão divididos em um unico arquivo que:  lida com as mensagens e timestamps e que permite aos usuários enviar e receber mensagens

## Abstract
This repository contains the source code and related resources for the Local Network Chat project. The project is a distributed chat system within a local network, allowing users to exchange real-time messages. The code is divided into three parts: a Python server that handles messages and timestamps, a Python client that enables users to send and receive messages. This solution aims to facilitate communication and interaction among users within a local network.

## Introdução
O projeto Chat em Rede Local visa fornecer uma plataforma de comunicação eficiente em um ambiente de rede local. Em um mundo cada vez mais conectado, a comunicação instantânea é essencial, e o objetivo é criar uma solução de chat que atenda a essa necessidade, permitindo que os usuários troquem mensagens de forma rápida e fácil em uma rede local.

## Fundamentação Teórica

Comunicação em Rede Local:

A comunicação em rede local refere-se à troca de informações entre dispositivos dentro de uma área geográfica restrita, como um escritório ou residência. O chat em rede local permite que os usuários se comuniquem de maneira eficiente e instantânea, sem depender de servidores externos.

Protocolo de Comunicação:

O projeto utiliza sockets e protocolo UDP para permitir a comunicação entre diferentes nós da rede local. O uso do protocolo UDP oferece vantagens, como velocidade e simplicidade, adequadas para uma aplicação de chat em tempo real.

## Metodologia
O projeto é dividido em duas funções principais:

Escuta de Chat: Uma Thread Python que gerencia as mensagens, timestamps e a ordem dos eventos no chat.
Cliente de Chat: Uma execução Python que permite aos usuários enviar e receber mensagens, garantindo uma experiência de chat em tempo real.
A operação começa com o usuário iniciando o cliente de chat, fornecendo um apelido (nick) e conectando-se ao servidor. A partir desse momento, os usuários podem enviar mensagens em tempo real, e o servidor mantém a ordem das mensagens para garantir uma conversa consistente.

## Para a execução do problema é necessário seguir estes passos abaixo

#### Executar o Código:
```
  pip install cryptography
```
```
  python3 chat.py
```

## Resultados e Discussões
O projeto de Chat em Rede Local demonstra que a comunicação em tempo real em uma rede local pode ser alcançada de maneira eficiente usando tecnologias como sockets e protocolo UDP. Essa solução pode ser implementada em ambientes onde a comunicação instantânea é fundamental, como escritórios ou residências. O aprimoramento contínuo pode incluir recursos adicionais e melhorias na experiência do usuário. 
Como a possível melhoria de terminar a exibição do histórico de mensagens pelo usuário mais antigo que está parcialmente implementado, faltando apenas puxar o histórico de mensagens assim que um novo usuário se conectar ao Mensageiro, sem que ele precise digitar comandos para puxar esse histórico de mensagens como está agora. Ou a confirmação de envio das mensagens e recebimento das mensagens o que garantiria a entrega e o recebimento das mensagens, fazendo um papel que o UDP não está acostumado a fazer. Isso garantiria que não haveria falhas de omissão de mensagens e que erros de envio e não recebimento seriam muito mais dificeis, além da organização das mensagens recebidas.

Autor
=======
| [<img src="https://avatars.githubusercontent.com/u/38389307?v=4" width=115><br><sub>Alexandre Silva Caribé</sub>](https://github.com/AlexandreCaribe) 
