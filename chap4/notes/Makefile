.PHONY: clean

NOTES = special_chars
INPUT = $(NOTES:=.tex)
OUTPUT = $(INPUT:.tex=.pdf)

all: $(OUTPUT)

clean:
	@latexmk -c
	@rm -f *.bbl *.cpt

cleanall: clean
	@rm -f *.pdf
	
%.pdf: %.tex
	@latexmk -pdf $?
