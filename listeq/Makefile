.PHONY: listeq.pdf

default: listeq.sty listeq.pdf

listeq.sty:
	tex listeq.ins

listeq.pdf: listeq.sty
	pdflatex -shell-escape listeq.dtx
	pdflatex -shell-escape listeq.dtx
	makeindex -s gind.ist -o listeq.ind listeq.idx
	makeindex -s gglo.ist -o listeq.gls listeq.glo
	pdflatex -shell-escape listeq.dtx
	pdflatex -shell-escape listeq.dtx

clean:
	-rm listeq.aux listeq.glo listeq.gls listeq.idx listeq.ilg
	-rm listeq.ind listeq.log listeq.out listeq.sty listeq.toc
	-rm example.out
	-rm -R _minted-listeq/
