BIB=references.bib
DOC=Report
TEX=$(DOC).tex
BIBTEX=bibtex
LATEX=pdflatex



# Stages:
# Make report
# Compile referances
# Insert referances
# Update page numbers if necessary
all: $(TEX) $(BIB)
	$(LATEX) $(TEX); $(BIBTEX) $(DOC); $(LATEX) $(TEX);$(LATEX) $(TEX);


# All that exist
.PHONY: clean
clean:
	rm -f $(DOC).bbl $(DOC).dvi $(DOC).aux $(DOC).blg $(DOC).log
