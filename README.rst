===========================
Compilando os arquivos .tex
===========================

Este trabalho de conclusão de curso foi feito utilizando LaTeX [#]_ , seguindo (ou pelo menos tentando) as orientações gerais para construção de trabalhos monográficos do Instituto Federal Fluminense (IFF).

Pré requisitos
==============

Para compilar os arquivos .tex é necessário a instalação do pacote *abntex*. Para isso, basta executar o seguinte comando em um terminal:

	$ sudo apt-get install abntex

Gerando arquivos .pdf a partir dos arquivos .tex
================================================

Dica retirada do GitHub do Quali-Ágil [#]_. O *latexmk* [#]_ é um script que agiliza o processo de criação do arquivo .pdf de um determinado arquivo .tex pois não se torna necessário executar os comandos *latex* e *bibtex* repetida vezes.


Instalando o *latexmk*
======================

As únicas dependências do *latexmk* são o *TeX*, *LaTeX* e *Perl*.

Para instalar o script, bastar executar em um terminal:

    $ sudo cp latexmk.pl /usr/bin/latexmk
    
    $ sudo chmod a+rx /usr/bin/latexmk
    
Usando o *latexmk*
==================

Para gerar um .pdf a partir de um .tex utilizando o script, basta apenas executar em um terminal:

    $ latexmk -pdf nome_do_arquivo.tex

.. [#] http://www.latex-project.org/
    
.. [#] http://github.com/qualiagil

.. [#] http://www.phys.psu.edu/~collins/software/latexmk-jcc/
