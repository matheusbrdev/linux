# sudo, locate, updatedb e which

## locate

- Uso:

  - ```bash
    $ locate nomeDesejado
    ```

    > Isto lhe trará todas as ocorrências(localização) do nome passado por parâmetro no HD e no seu sistema

## sudo

- Uso:

  - ```bash
    $ sudo comando
    ```

    > Executa o comando ou instrução passada como parâmetro no modo super user.

## updatedb

> O 'locate' retorna os dados de um db interno do OS, para atualizar este db use o updatedb.

- Uso:

  - ```bash
    $ sudo updatedb
    ```

## which

> prendemos anteriormente como buscar por arquivos e programas no sistema operacional com o comando `locate`, Porém o Terminal retorna uma lista extensa de arquivos que possuem em  seu nome, parte do texto que usamos para pesquisar. Mas, qual é o  arquivo que será executado quando digitamos o comando `vi`, `gedit` ou mesmo o `firefox`?
>
> Para saber onde os programas estão instalados usamos o comando ``which``

- Uso: 

  - ```bash
    $ which alvoASerProcurado
    ```

    > Exemplo:

    ```bash
    $ which firefox
    ```

    > Resultado: /usr/bin/firefox 
