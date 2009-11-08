LATEX = /usr/share/texmf/bin/latex
PDFLATEX = /usr/share/texmf/bin/pdflatex
BIBTEX = /usr/share/texmf/bin/bibtex


TARGET=seg_info_contratos
TRASH = *.aux *.log *.toc *~ *.blg *.bbl
RM = /usr/bin/rm


pdf:
	$(PDFLATEX) $(TARGET)
	$(BIBTEX) $(TARGET)
	$(PDFLATEX) $(TARGET)
	$(PDFLATEX) $(TARGET)

clean:
	$(RM) $(TRASH)

clean-all: clean
	$(RM) *.pdf

