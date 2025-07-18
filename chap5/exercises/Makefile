.PHONY: clean

EXERCISES = ex8 ex9 ex10 ex11 ex12 ex13 ex14
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
