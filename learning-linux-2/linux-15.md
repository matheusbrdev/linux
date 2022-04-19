# SSH

No ssh existe o cliente e o servidor. O cliente seria para conectarmos em uma máquina com ssh e o servidor seria para que outras máquinas se conecte a minha.

Para instalar os dois user:

```bash
$ sudo apt install ssh
```

### Para se conectar a uma máquina a partir do ssh:

```bash
$ ssh nomeDeUsuário@ip
```

> Neste tipo de acesso só temos contato com o terminal. Para termos a possibilidade de acesso gráfico a partir do terminal usamos: 
> 
> ```bash
> $ ssh -X nomeDeUsuário@ip
> ```

### Copiar um arquivo da minha máquina local para a remota:

```bash
$ scp -r arquivo nomeDeUsuário@ip:~/(diretório)
```
