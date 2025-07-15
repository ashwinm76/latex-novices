.PHONY: clean

NOTES = grouping
INPUT = $(NOTES:=.tex)
OUTPUT = $(INPUT:.tex=.pdf)

all: $(OUTPUT)

clean:
	@latexmk -c
	@rm -f *.bbl *.cpt *.synctex.gz

cleanall: clean
	@rm -f *.pdf
	
%.pdf: %.tex
	@latexmk -pdf $?
