# PS1

Já vimos que com o devido cuidado, podemos alterar nossas variáveis  de ambiente para customizar a forma de interação com o nosso terminal.

Uma outra variável de ambiente é a `PS1`. Vamos olhar o conteúdo dela:

```bash
$ echo $PS1
\[\e]0;\u@\h: \w\a\]${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[00m\]\$
```

Quando estamos utilizando o terminal, algumas informações sempre são mostradas, exemplo: `lucas@lucas-Inspiron-5458:~$`. Essa formatação é definida na variável `PS1`.

Experimente alterar a variável e perceba que a definição do seu prompt será alterada:

```bash
lucas@lucas-Inspiron-5458:~$ PS1="alura>"
alura>
alura>PS1="alura:"
alura:
```

