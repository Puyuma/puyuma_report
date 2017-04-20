all:	paper.pdf

paper.pdf: paper.tex
	pdflatex $^
	bibtex paper >/dev/null || echo
	pdflatex $^ 2>/dev/null >/dev/null
	pdflatex $^

edit:
	texmaker paper.tex &

clean:
	rm -f *.dvi *.aux *.log *.ps *.pdf *.out paper.bbl paper.blg
