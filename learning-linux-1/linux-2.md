## Manipulando, compactando e descompactando

- Comando 'cp': 
	+ Copiando arquivo:
		*  ``$ cp arquivoAserCopiado nomeDacopia(com extensão)``
	+ Para copiar diretórios: 
		* ``$  cp -r diretorioAserCopiado diretorioCopia``
		
- Comando 'mv': 
	+ Mudando o nome do arquivo:
		* ``$ mv arquivoAterNomeMudado novoNomeDoArquivo ``
	+ Movendo de diretório: 
		* ``$ mv arquivoAserMovido novoDiretorio/(pode renomear ao mesmo tempo se quiser) ``
		
### Compactando:
- Compactando diretório:
	+ ``$ zip nome.zip diretorioAserCompactado``
	+ Diretório e itens dentro:
		* ``$ zip -r nome.zip diretorioAserCompactado``

### Descompactando: 
- Verificando o que há dentro de um arquivo compactado:
	+ ``$ unzip -l arquivoZipado``
- Descompactando:
	+ ``$ unzip arquivoCompactado``
	+ Use o '-q' quando não quiser ver as infos da descompactação:
		* ``$ unzip -q arquivoCompactado``