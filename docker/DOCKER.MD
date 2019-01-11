# **DOCKER**

**Documento de instalação do DOCKER**

| **AUTOR** | **VERSÃO** | **DATA** | **COMENTÁRIOS** |
| --- | --- | --- | --- |
| Danilo R. Dias | 1.0 | 04/01/2019 | Criação do documento |

* [Windows](#Windows)
* [Linux](#Linux)  
* [MacOS](#MacOS)
* [Alternativa](#Alternativa)

____

## O Docker Toolbox

Vai instalar tudo que é necessário para que você possa trabalhar com o Docker em seu computador, pois ele irá instalar também a `Oracle VirtualBox`, a máquina virtual da Oracle que vai permitir executar o Docker sem maiores problemas.

# Instalação

## Windows
Primeiramente você deve se atentar aos requisitos do uso do `Docker for Windows`, ou seja, deve possuir um Windows com:

* Arquitetura 64 bits
* Versão Pro, Enterprise ou Education.
* Virtualização habilitada (Gerenciador de Tarefas, e indo na aba Perfomance)

Na página do [Docker for Windows](https://store.docker.com/editions/community/docker-ce-desktop-windows), baixe o instalador clicando [aqui](https://download.docker.com/win/stable/InstallDocker.msi). 
Siga o passo a passo do instalador para aceitar a licença, autorize o instalador e siga com a instalação. 
Ao clicar em Finish, encerre a sessão do Windows e inicie-a novamente. Ao fazer o login, habilitar o `Hyper-V`, clicando em `Ok`, para que o computador seja reiniciado.

Quando o computador terminar a reinicialização, irá aparecer um ícone do Docker na barra inferior, à direita, ao lado do relógio. 

O Docker pode demorar um pouco para inicializar, mas quando a mensagem Docker is running for exibida, significa que ele foi instalado com sucesso e você já pode utilizá-lo.

## Instalando com Docker Toolbox
Para instalar baixe-o [aqui](https://download.docker.com/win/stable/DockerToolbox.exe).

____

## Linux
Preparando o ambiente: Instalando Docker no Ubuntu

Docker no Ubuntu 64 bits. Todos os comandos listados devem ser executados no seu terminal.

`Antes de mais nada, remova possíveis versões antigas do Docker:`

```
sudo apt-get remove docker docker-engine docker.io
```
Depois, atualize o banco de dados de pacotes:
```
sudo apt-get update
```
Agora, adicione ao sistema a chave GPG oficial do repositório do Docker:
```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
```
Adicione o repositório do Docker às fontes do APT:
```
sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
```
Atualize o banco de dados de pacotes, pare ter acesso aos pacotes do Docker a partir do novo repositório adicionado:
```
sudo apt-get update
```
Por fim, instale o pacote docker-ce:
```
sudo apt-get install docker-ce
```
Caso você queira, você pode verificar se o Docker foi instalado corretamente verificando a sua versão:
```
sudo docker version
```
E para executar o Docker sem precisar de sudo, adicione o seu usuário ao grupo docker:
```
sudo usermod -aG docker $(whoami)
```
____

## MacOS
Primeiramente você deve se atentar aos requisitos do uso do Docker for Mac, ou seja, deve possuir um macOS:

* Modelo 2010 ou mais recente
* Versão OS X El Capitan 10.11 ou mais recente
* Com no mínimo 4GB de memória RAM
* Sem VirtualBox instalada na versão 4.3.30 ou anterior, pois causa incompatibilidade com o Docker

A página dos requisitos pode ser acessada [aqui](https://docs.docker.com/docker-for-mac/install/#what-to-know-before-you-install).

Baixe o instalador clicando [aqui](https://download.docker.com/mac/stable/DockerToolbox.pkg).

Instale o Docker, clicando no `.dmg` baixado anteriormente e arrastando o Docker para as aplicações. Após isso, pesquise pelo Docker, confirme que quer utilizá-lo e dê acesso privilegiado a ele, clicando em OK e digitando a senha de administrador em seguida.

No menu superior do `macOS`, à direita, o ícone do Docker aparecerá. Ele pode demorar um pouco para inicializar, mas quando a mensagem Docker `is now up and running!` for exibida, significa que ele já pode ser utilizado.

## Instalando com Docker Toolbox
Para instalar baixe-o [aqui](https://download.docker.com/mac/stable/DockerToolbox.pkg).

____

## Alternativa

## Utilizando o Play With Docker

Não se desespere caso você tenha tido algum problema em instalar o Docker em sua máquina, você também tem a opção de utilizar o [Play With Docker](https://labs.play-with-docker.com/).

Nele você poderá utilizar os comandos vistos daqui em diante e testar as diversas funcionalidades que o Docker proporciona. Ao acessar o site basta clicar em +Add New Instance e começar a utilizá-lo como estivesse usando sua máquina normalmente.