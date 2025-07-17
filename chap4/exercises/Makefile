.PHONY: clean

EXERCISES = ex1 ex2 ex3 ex4 ex5 ex6 ex7
INPUT = $(EXERCISES:=.tex)
OUTPUT = $(INPUT:.tex=.pdf)

all: $(OUTPUT)

clean:
	@latexmk -c
	@rm -f *.bbl *.cpt *.synctex.gz

cleanall: clean
	@rm -f *.pdf
	
%.pdf: %.tex
	@latexmk -pdf $?
