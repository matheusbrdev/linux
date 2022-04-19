# Instalação a partir do código fonte

Geralmente o código fonte vem compactado com tar.gz. Para descompactar use: 

```bash
$ tar zxf nomeDoArquivoCompactado
```

> Usa-se tar.gz para compactar esse tipo de arquivo porque essa compactação mantém suas permissões de execução.

### Pontos importantes para a instalação:

1. Testar se a nossa máquina atende os requisitos para instalação.
   
   - Para isso existe um script chamado 'configure'. Para executá-lo certifique-se que está dentro da pasta descompactada e digite:
     
     ```bash
     $ ./configure
     ```

### Para rodar o build do projeto:

```bash
$ make
```

> Dentro da pasta do projeto.
> 
> Caso de algum erro de dependência... procure a dependência com o apt e instale.

### Depois do make

Após gerar o build do projeto, user para instalar:

```bash
$ sudo make install
```
