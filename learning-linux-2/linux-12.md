# Instalando .deb

- Uso: 

  - ```bash
    $ sudo dpkg -i arquivo.deb
    ```

    > -i é o parâmetro passado para informar instalação

  - Para remover um pacote instalado com dpkg:

    - ```bash
      $ sudo dpkg -r nomeDoPacote
      ```



# Questão 

Como podemos instalar o arquivo 'google-chrome-stable_current_amd64.deb' no nosso sistema?

- Resposta: 

  - ```bash
    $ sudo dpkg -i google-chrome-stable_current_amd64.deb
    ```

  > Obs:
  >
  > No caso do Google Chrome, iremos receber alguns erros, pois o pacote depende de outros pacotes e o `dpkg` não resolveu isso pra gente. Para baixar as dependências e fazer com que o Google Chrome funcione corretamente, pedimos para o `apt-get` tentar resolver esse problema:
  >
  > ```bash
  > $ sudo apt-get -f install
  > ```

