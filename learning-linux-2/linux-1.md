# Kill, ps e grep 

### ps:

- Uso: 

  - ```bash
    $ ps
    ```

    > Exibe os processos que estão rodando no próprio terminal.
    
  - Ou pstree 

    - ```bash
      $ pstree
      ```

      > Exibe os processos em árvore

- Parâmetros:

  - -e

    - ```bash
      $ ps -e
      ```

      > Exibe todos os processos do SO.

  - -ef

    - ```bash
      $ ps -ef 
      ```

      > Exibe todos os processos do SO com informações a mais sobre os mesmos.

### kill:

- Uso: 

  - ```bash
    $ kill numeroDoPID
    ```

    > Isto irá matar o processo referente ao número do PID passado por parâmetro.

- Parâmetros:

  - -9:

    - ```bash
      $ kill -9 numeroDoPID
      ```

      > Morte do processo forçada.

### grep:

- Uso:

  - ```bash
    $ grep nome
    ```

    > Filtra linhas pelo nome passado por parâmetro.
    > Geralmente é mais usado com outros programas como o 'ps'



### OBS:

É possível juntar programas com o ' | '. Exemplo: 

```bash
$ ps -ef | grep firefox
```

> Irá trazer apenas a ocorrência de execução do processo do firefox no SO.

Outro exemplo seria:

```bash
$ cat arquivo.txt | grep teste
```

> Irá me trazer apenas as linhas do arquivo onde aparece a palavra 'teste'.