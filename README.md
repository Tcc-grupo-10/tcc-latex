#TCC Latex
####Algoritmo de Processamento de Linguagem Natural para Análise de Sentimento em Mídias Sociais

####Como Compilar: Linux

* Instalar todas as dependências do latex, abntex
	* TODO: Descrever melhor
	
* Usando o Texmaker para compilar:
	* Opções -> Configurar -> Compilar -> Usuário -> Colar código abaixo:
	* ```pdflatex -synctex=1 -interaction=nonstopmode %.tex|bibtex %.aux|pdflatex -synctex=1 -interaction=nonstopmode %.tex|makeglossaries %|pdflatex -synctex=1 -interaction=nonstopmode %.tex|evince %.pdf```
	* Este irá ```makeGlossaries``` + ```pdfLaTeX``` + ```Bibtex``` + ```pdfLaTeX(2x)``` + ```viewPDF``` 

### Latex Hacks
* Usar aspas: crase_crase_TEXTO_apostrofe_apostrofe: 
	* ``` ``TEXTO'' ```
* Glossário: 
	* Adicionar item no glossaires.tex seguindo o padrão:
		* ```\newacronym{label}{sigla}{significado}```
	* usar ```\gls{label}``` no texto