# Template para desenvolvimento e entrega de NAC

Esse é um guia simples, o grupo pode e deve modificar o template conforme necessidade. 

# Nome do projeto

**nome dos alunos: CATARINA HENRIQUES CAMUSSI   RM87553** 

**Turma: 2TDSG**

**Ano:2022**

## Objetivo / descrição do Projeto

Sobre o projeto:
Conectamos um sensor de umidade no arduíno e mostramos na tela a informção contendo a umidade do local em tempo real utilizando dashboards, o node red para criar o fluxo e bibliotecas como o arduinojson. 
Utilizamos o  protocolo MQTT , então qualquer pessoa de qualquer parte do mundo , pode fazer ter acesso a esses dados em tempo real. 

Conectamos o arduíno a um sistema de RfID , que quando o usuario encosta seu cartão/ tag rfid , é disparado uma mensagem no telegram informando que alguém entrou usando a tag rfid e mostra em forma de json o valor. 

Através da ferramenta do botfather (nativa do telegram), conectei o bot do telegram com o fluxo de umidade feito no node-red, porém o telegram não estava mandando o valor da umidade e sim uma mensagem estática , por isso foi retirado do nó , mas para implementar basta usar um reciver , um sender , uma function e um debug e dentro da function colocar: msg.payload.content = "sua mensagem"; e claro colocar as credenciais do seu bot no sender e no reciver. 

## Diagrama do projeto

Adicione uma ou mais fotos do projeto, pode ser uma imagem da arquitetura, do circuito eletrônico do Flow desenvolvido. 

<img src="/cp4.png" width="550">


## Como usar 

instalar no arduino a lib ArduinoJson , no node red a lib: node-red dashboard e node red telegram-bot
* Pode ser utilizado marcadores
* Para ajudar na formatação

## Vídeo no youtube , mostrando funcionamento do servo motor antes de corroper o arqivo .json   https://youtu.be/H-cWkc-SPF0



### Referências 

* [mastering-markdown](https://guides.github.com/features/mastering-markdown/)
* [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
