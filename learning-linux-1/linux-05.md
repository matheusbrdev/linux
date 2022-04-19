# Edição de arquivos com Vi

O **vi** é um editor de texto do sistema operacional Unix e semelhantes. Esta presente em práticamente todas as versões do **Linux**. Para quem sabe como utilizar é um ótimo editor com vários recursos.

- Uso: 

  - ```bash
    $ vi nomeDoArquivo(.txt, .md, etc)	
    ```

    > Por padrão ele abre o arquivo no modo de vizualização apenas, para inserir ou remover conteúdos basta alterar o modo presionando a letra referente.

  - modos: 

    - ' i ' modo de inserção(começando antes de onde está o cursor);
    - 'a' modo de inserção(começando depois de onde se está o cursor);
    - 'x' remove caracteres;
    - 'dd' remove uma linha inteira;

    > Para sair de um modo... use 'Esc'

  - Comandos: 

    > Para poder digitar um comando precione ':'

    - 'w' para salvar;
    - 'q' para sair.

  - Atalhos:

    - 'G' vai para última linha;

      > Para ir a outras linhas específicas adicione o número da linha ao G, assim: '3G'

    - '$' vai para o final de uma linha;

    - '0' vai para o começo da linha;

    - '/' para pesquisar;

      > Vai para a primeira ocorrência desta palavra. Para ir a próxima ocorrência use: 'n' e para voltar use: 'N'

    - 'yy' copia uma linha;

    - 'p' cola;