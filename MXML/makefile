PDFLATEX = pdflatex
BIBTEX = bibtex
TEXFILE = hk_perfect_binary_trees

all: $(TEXFILE).pdf

$(TEXFILE).pdf: $(TEXFILE).tex
	$(PDFLATEX) $(TEXFILE)
	$(BIBTEX) $(TEXFILE)
	$(PDFLATEX) $(TEXFILE)
	$(PDFLATEX) $(TEXFILE)

clean:
	rm -f *.aux *.bbl *.blg *.log *.out *.pdf

.PHONY: all clean