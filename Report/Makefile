BIB=references.bib
RER=Report
TEX=$(RER).tex
BIBTEX=bibtex
LATEX=pdflatex



# Stages:
# Make report
# Compile referances
# Insert referances
# Update page numbers if necessary
all: $(TEX) $(BIB)
	$(LATEX) $(TEX); $(BIBTEX) $(REP); $(LATEX) $(TEX);$(LATEX) $(TEX);


# All that exist
.PHONY: clean
clean:
	rm -f Report.bbl Report.dvi Report.aux Report.blg Report.log
