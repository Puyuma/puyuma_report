PAPER_NAME = puyuma

all:	$(PAPER_NAME).pdf

$(PAPER_NAME).pdf: $(PAPER_NAME).tex
	pdflatex $^
	bibtex paper >/dev/null || echo
	pdflatex $^ 2>/dev/null >/dev/null

edit:
	texmaker $(PAPER_NAME).tex &

clean:
	rm -f *.dvi *.aux *.log *.ps *.pdf *.out $(PAPER_NAME).bbl $(PAPER_NAME).blg
