.PHONY: all clean

all: endocytosis.pdf view

endocytosis.pdf: endocytosis.tex equations.tex endocytosis.bib
	latexmk -pdfps -pdflatex="pdflatex --shell-escape %O %S" $<

view: 
	evince endocytosis.pdf &

##########################################################################3

clean:
	latexmk -C
