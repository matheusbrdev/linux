## Mais sobre compactação e descompactação.


> No mundo linux temos outros 'tipos' de compactação.
> como por exemplo: tar.gz.

> Por padrão ele faz a compactação e descompactação de forma silenciosa. Para executar essas tarefas tendo mais infos sobre o processo, use 'v' também como parâmetro. Exemplo: ``$ tar -vxzf  ``

- Para compactar com 'tar': 
	+ ``$ tar -cz alvoAserCompactado > nomeParaASaídaCompactada.tar.gz``
	> Obs:
	> - no comando acima o 'c' vem de 'create' e o 'z' vem de 'zip', ou seja, criar o tar e comprimir;
	> - A compactação com tar já é recursiva por padrão e por isso não é necessário usar o parâmetro '-r'. 
	+ Outra opção é: 
		* ``$ tar -czf nomeParaASaídaCompactada.tar.gz alvoASerCompactado ``
		> O 'f' trás a possibilidade de definir o nome da saída sem precisar redirecionar com '>'
	
	
- Para descomparctar compressões com 'tar.gz':
	+ ``$ tar -xz < entradaCompactada.tar.gz``
	> Obs:
	> - no comando acima o 'x' vem de 'extract' e o 'z' vem de 'zip', ou seja, extrair o tar comprimido;

	+ Outra opção é: 
		* ``$ tar -xzf nomeDaEntradaCompactada.tar.gz ``
		> O 'f' trás a possibilidade de definir o nome da saída sem precisar redirecionar com '<'.
		
## bzip2:

Vimos que o comando tar não compacta, apenas empacota os arquivos. E que podemos utilizá-lo em conjunto com outros compactadores. Vimos como compactar no formato ``.gz``, que é o formato gerado pelo compactador gzip.

Um outro formato de compactação que podemos utilizar junto com o tar é o formato ``.bzip2``. Esse formato é mais eficiente na compactação, conseguindo criar arquivos menores. Porém o tempo que o ``.bzip2`` leva para criar o arquivo compactado é maior do que o tempo do gzip.

Para criar um arquivo .tar compactado com o bzip2, substituímos o -z (de gzip) por um -j. O formato que utilizamos é o .tar.bz2.

Exemplo:

``$ tar -cjf nomeParaAsaídaCompactada.tar.bz2 alvoAserCompactado``