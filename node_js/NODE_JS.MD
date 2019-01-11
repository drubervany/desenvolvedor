# **NODE JS**

**Documento de instalação do NodeJs**


| **AUTOR** | **VERSÃO** | **DATA** | **COMENTÁRIOS** |
| --- | --- | --- | --- |
| Danilo R. Dias | 1.0 | 04/01/2019 | Criação do documento |

* [Windows](#Windows)
* [Linux](#Linux)  
* [MacOS](#MacOS)
* [Documentação](#Documentação)


____

# Instalação

## Windows
Disponível diretamente da página do Node.js:

Download:
[32 bits](https://nodejs.org/dist/latest-v10.x/node-v10.13.0-x86.msi) ou 
[64 bits](https://nodejs.org/dist/latest-v10.x/node-v10.13.0-x64.msi) para Windows.

Baixe e execute o instalador (arquivo.msi). 

`Não troque a pasta padrão do Node.js, a não ser que saiba exatamente o que está fazendo`

`Atenção:` na plataforma Windows, dependendo da configuração da sua máquina, ou do uso de uma rede corporativa (proxy), pode ser que a instrução npm install não funcione. Caso isso aconteça, pode-se tentar os passos a seguir. _Caso o primeiro funcione,_ **não é necessário fazer o segundo**:

`1) Problema no certificado:` no terminal, deve-se executar o comando npm set strict-ssl false. Em seguida, é possível repetir a operação de instalação que falhou.

`2) Redes de empresa ou proxy da rede:` alguns usuários acessam a rede através de um proxy. Isso pode impedir que o npm tenha acesso ao seu repositório. Nesse sentido, é necessário saber o endereço do proxy para então configurá-lo através das instruções a seguir (troque proxy.company:8080 pelo endereço do seu proxy).

```
npm config set proxy http://proxy.company.com:8080
npm config set https-proxy http://proxy.company.com:8080 
```
____


## Linux
No `Ubuntu`, através do terminal (permissão de administrador necessária) executemos o comando abaixo:
```
sudo apt-get install -y nodejs
```

Em algumas distribuições Linux, pode haver um conflito de nomes quando o Node é instalado pelo `apt-get`. Neste caso específico, no lugar do binário ser node, ele passa a se chamar `nodejs`. Isso gera problemas pois, como a instrução `npm start` procura o binário node, e não nodejs, ela não funcionará. Para resolver, usemos a seguinte instrução no terminal para subir o servidor:

```
nodejs server
```
Ou no Ubuntu:
```
sudo ln -s /usr/bin/nodejs /usr/bin/node
```
____

## MacOS
Usar o gerenciador de pacotes `pip`, do mundo Python, para instalar o AWS CLI.

O [Homebrew](http://brew.sh/index_pt-br.html), é a maneira mais recomendada para instalar o Node.js, por meio do comando:

```
brew update
brew install node
```

Não usa `homebrew`? Sem problema, basta baixar o instalador clicando no botão install, diretamente da página do [Node.js](https://nodejs.org/en/).

## Documentação

A documentação fornece informações detalhadas sobre as funções ou objetos no Node.js

NodeJs: https://nodejs.org/en/docs/