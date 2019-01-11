# **AWS CLI**

**Documento de instalação do AWS CLI**


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
Disponível na página inicial do [AWS CLI](https://aws.amazon.com/pt/cli/)

Para baixar diretamente aqui a versão de 
[32 bits](https://s3.amazonaws.com/aws-cli/AWSCLI32.msi) ou 
[64 bits](https://s3.amazonaws.com/aws-cli/AWSCLI64.msi) para Windows.

Baixe e execute o instalador (arquivo.msi). Depois abra o Prompt de Comando e execute o comando aws:
![prompt](\img\windows\prompt.png)

____


## Linux
Usar o gerenciador de pacotes `pip`, do mundo `Python`, para instalar o `AWS CLI`.

Instalar o Python, execute o seguinte comando no seu terminal:
```
sudo apt-get update
sudo apt-get install python3
```

Agora baixe o [get-pip.py](https://s3.amazonaws.com/caelum-online-public/617-aws-s3/03/arquivos/get-pip.py), responsável por instalar o gerenciador de pacotes pip. Ao baixá-lo, execute pelo terminal:
```
sudo python get-pip.py
```

Verifique no seu terminal versão do Python 
```
python -V
```

Podemos usar o gerenciador de pacotes pip para baixar e instalar o AWS CLI:
```
sudo pip install awscli
```

Execute o comando aws:
![prompt](\img\linux\cli-linux.png)

____

## MacOS
Usar o gerenciador de pacotes `pip`, do mundo Python, para instalar o AWS CLI.

Instalar o `Python 3` no macOS, temos duas opções, através do [Homebrew](http://brew.sh/index_pt-br.html), fazemos:
```
brew update
brew install python3
```

caso você não utilize o `Homebrew`, baixe o instalador do Python através do seu [site oficial](https://www.python.org/downloads/)

Verifique no seu terminal versão do Python 
```
python -V
```

Podemos usar o gerenciador de pacotes pip para baixar e instalar o `AWS CLI`:
```
sudo pip install awscli
```

Execute o comando aws:
![prompt](\img\macOS\cli-mac.png)

## Documentação

O `AWS Command Line Interface` User Guide orienta você durante a instalação e configuração da ferramenta. Depois disso, você pode começar a fazer chamadas para seus serviços AWS pela linha de comando. 

AWS CLI: https://aws.amazon.com/pt/cli/