# Killall e top

### top

- Uso: 

  - ```bash
    $ top
    ```

    > Exibe o uso do hardware pelos processos.

### killall

- Uso:

  - ```bash
    $ killall nome
    ```

    > Mata todos os processos com o nome igual ao passado por parâmetro.



### Obs

O top possui algumas opções que podemos utilizar para alterar a forma padrão de como as informações são mostradas.

Para mostrar apenas os processos de um determinado usuário, podemos utilizar a opção `-u`:

```bash
top -u lucas
```

Para acompanhar as informações de um processo específico, podemos utilizar a opção `-p` passando como argumento o `PID` do processo:

```bash
$ ps -e | grep firefox
19509 ?        00:00:03 firefox
$ top -p 19509
```

Por padrão, o `top` atualiza a tela com novas informações sobre os processos a cada 3 segundos. Para alterar esse tempo basta pressionar `d` enquanto estiver rodando o `top`, inserir o valor desejado e pressionar a tecla `Enter`

