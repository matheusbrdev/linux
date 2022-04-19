# Trabalhando com grandes arquivos de texto

### head:

- Uso:

  - ```bash
    $ head nomeDoArquivo.txt
    ```

    > Isso lhe trará as 10 primeiras linhas.
    >
    > Para lhe trazer o número de linhas desejado use '-n numeroDeLinhas', exemplo:

    ```bash
    $ head -n 3 nomeDoArquivo.txt
    ```



### tail:

- Uso:

  - ```bash
    $ tail nomeDoArquivo.txt
    ```

    > Isso lhe trará as 10 últimas linhas.
    >
    > Os mesmos parâmetros para retornar um número de linhas desejado no comando 'head' se aplicam aqui no 'tail'.



### less:

- Uso: 

  - ```bash
    $ less nomeDoArquivo.txt
    ```

    > Isto lhe trará o arquivo sob demanda. Ao tempo que desce na navegação ele traz as linhas.
    >
    > Use: 'j' para descer, 'k' para subir e 'q' para sair. 