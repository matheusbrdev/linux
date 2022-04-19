# wc

O comando `wc` pode ser utilizado para contar o número de  palavras, caracteres e linhas que um arquivo possui. Junto com o wc  podemos utilizar a opção `-w` para indicar que desejamos contar apenas o número de palavras que existem no arquivo. O `*.txt` indica que desejamos realizar a contagem em todos os arquivos `.txt` do nosso diretório atual.

```
$ wc -w *.txt
 6 projetos_java.txt
10 projetos_php.txt
16 total
```

Além de contar o número de palavras em um arquivo, o comando `wc` pode também contar o número de caracteres e linhas em um arquivo, ou em uma saída do terminal. Para isso, podemos utilizar a opção `-c` para caracteres e `-l` para linhas.

Se utilizarmos o comando `ps -e`, que lista todos os processos, podemos passar o retorno do `ps` para o `wc -l` contar quantas linhas o retorno possui. A quantidade de linhas  representa a quantidade de processos existentes no nosso sistema.

```bash
$ ps -e | wc -l
```

