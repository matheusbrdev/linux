# adduser e chmod

## adduser

- Uso:

  - ```bash
    $ adduser nomeDoUsuario
    ```

    > Isto irá adicionar um novo usuário com o nome passado por parâmetro.  Vai também pedir a senha deste novo user.
    > OBS: Você deve estar em user root para executar este comando. 
    >
    > - O user root tem acesso a todos os usuários sem pedir senha.
    > - Por padrão os usuários tem permissão de leitura da home de outros usuários.

## chmod

Se verificarmos as permissões dos diretórios pessoais de cada usuário usando o comando `ls -l` no diretório '/home', teremos:

![permissões para os diretórios pessoais em /home](https://s3.amazonaws.com/caelum-online-public/linux2/a7v1-home-users.png)

Veremos que para o diretório `jose` como usuário `jose` temos todas as permissões, execução e leitura para os usuários do mesmo grupo e execução e leitura para outros usuários. O que queremos é que  os outros usuários não tenham permissão alguma. Para tirarmos tais  permissões para os outros usuários, usamos o comando `chmod` da seguinte forma:

```bash
$ chmod o-rx jose
```

 Neste caso, o comando `chmod` é seguindo de alguns operadores, que são: `o` para *others*, ou seja, outros usuários, o `-` indica uma remoção de permissão, o `r` e `x` indicam permissões de leitura e execução. Se quiséssemos tirar permissões do próprio usuário, seria: `u-rx` e para o grupo seria: `g-rx`.

Agora se verificarmos novamente, veremos que o diretório do usuário `jose` não permite mais nenhuma operação para outros usuários:

![outros usuários sem permissão](https://s3.amazonaws.com/caelum-online-public/linux2/a7v1-jose-nenhuma-o.png)

​				                       