#

main = main
TEXFILES = $(addprefix ./, *.tex)
BIBFILE = bibliography.bib

$(main).pdf: $(main).tex $(TEXFILES) $(BIBFILE) Makefile
	pdflatex $(main)
	bibtex $(main)
	pdflatex $(main)
	pdflatex $(main)
        
clean:
	rm *.aux *.dvi *.pdf *.log *.blg *.out *.bbl *.toc *.lof
