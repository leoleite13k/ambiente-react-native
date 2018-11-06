Para configurar o ambiente Android no Linux, vamos precisar instalar 3 dependências: Node e JDK.

Certifique-se que você tenha o cURL instalado executando o seguinte comando no terminal:

```sh
sudo apt-get install curl
```

Agora com o cURL instalado, vamos instalar no NodeJS utilizando os seguintes comandos:

```sh
curl -sL https://deb.nodesource.com/setup_10.x | sudo bash -
sudo apt install nodejs
```

*Caso você não esteja em distribuições Debian/Ubuntu, siga os passos para instalação de acordo com seu sistema: https://nodejs.org/en/download/package-manager*

Com o NodeJS instalado, podemos instalar o CLI (Command Line Interface) do React Native:

```sh
sudo npm install -g react-native-cli

// Ou yarn global add react-native-cli
```

Agora precisamos instalar a JDK (Java Development Kit) na versão 8 ou maior com o seguinte comando:

```sh
sudo add-apt-repository ppa:openjdk-r/ppa
sudo apt-get update
sudo apt-get install openjdk-8-jdk
```

Podemos testar a instalação do JDK com o seguinte comando:

```sh
java -version
```

Em grande parte das vezes precisamos instalar algumas bibliotecas da versão 32bits do Linux para conseguir emular nosso projeto e para isso vamos utilizar o seguinte comando:

```sh
sudo apt-get install gcc-multilib lib32z1 lib32stdc++6
```