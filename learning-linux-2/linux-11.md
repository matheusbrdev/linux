# apt

Nesta aula vamos aprender como instalar um programa via Terminal de Linux. Como exemplo, iremos instalar um servidor FTP.

O Ubuntu nos disponibiliza um sistema de gerenciamento de pacotes chamado **apt**. Para ver as versões atualizadas dos programas que estão disponíveis para instalação fazemos:

```bash
$ sudo apt-get update
```

> Obs: A opção ``upgrade`` do `apt-get`, serve para atualizar todo o nosso sistema, atualizando as versões dos pacotes que já estão instalados.
>
> A opção `show` do comando `apt-cache`, mostra informações sobre um determinado pacote. Aproveite para fazer um teste:
>
> ```bash
> $ apt-cache show mysql-server-5.6
> ```

Veja que executamos o comando como *root* (`sudo`), isto porque esta é uma tarefa de administração, por isso é necessário que seja feita como *root*, caso não, teremos uma mensagem de permissão negada. Neste passo, o  Terminal irá buscar na internet o que existe de novidade nos programas  para instalação. Para buscar um programa de servidor FTP podemos fazer:

```bash
$ apt-cache search ftp
```

Este comando busca na lista de pacotes disponíveis, qualquer programa que se encaixe nesse termo de busca, por isso retorna uma longa lista de  programas. Sejamos mais restritos na busca e procuremos um servidor  específico:

```bash
$ apt-cache search vsftp
```

Como estamos usando uma busca mais restrita, poucos resultados serão  retornados pela busca, a imagem abaixo ilustra esses resultados.

![resultados de busca para vsftp](https://s3.amazonaws.com/caelum-online-public/linux2/a9v1-vsftp.png)

Achamos um bom servidor FTP, ele nos mostra o nome e uma curta descrição. Para instalar este programa fazemos:

```bash
$ sudo apt-get install vsftpd
```

## Removendo

Para que possamos remover programas, utilizamos o comando `apt-get remove` seguido do nome do programa. Como exemplo, vamos desinstalar o servidor que instalamos.

```bash
$ sudo apt-get remove vsftpd
```



## Resumo 

Aprendemos a instalar e desinstalar programas de forma fácil e prática com auxilio do gerenciador de pacotes `apt`. Os comandos são:

- `apt-get install`: instala um programa dado o nome
- `apt-get remove`: desinstala um programa dado o nome
- `apt-get update`: busca uma lista das versões atualizadas dos programas
- `apt-cache search`: procura os programas disponíveis para instalação