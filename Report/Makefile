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
	$(LATEX) $(TEX); makeglossaries $(DOC); $(BIBTEX) $(DOC); $(LATEX) $(TEX); $(LATEX) $(TEX);


# All that exist
.PHONY: clean
clean:
	ls $(DOC).* | grep -v "$(DOC)\.\(tex\)" | xargs -d"\n" rm
