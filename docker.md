# Docker commands
_____

```docker run```

Comando run sempre cria novos containers. Run é uma concatenação de quatros comandos docker:
* docker image pull, baixar a imagem do registry para maquina local 
* docker container create, criacao do container
* docker container start, inicializacao do conteiner
* docker container exec, execução do container no modo interativo
_____

```docker container ps```
* mostrar os containers em execução
_____

```docker container ps -a```
* mostrar todos os containers que foram executados independente do status
_____

```docker container run --rm debian ```
* remover container apos a execução
_____

```docker container run -it debian bash```
> ``` i ``` modo iterativo
> ``` t ``` terminal

* comando para entrar no terminal do container
_____

> Reutilização de container

``` docker container run --name mydeb -it debian bash ```
* Nomeando um container para reutiliza-lo
_____

``` docker container start -ai mydeb ```
> ``` a ``` atach, utilizar o container 
> ``` i ``` iterativo

* Qualquer arquivo modificado, criado, ou excluido. Com estes comandos ele ficara salvo no container porque se esta reutilizando o container e não criando um novo
_____