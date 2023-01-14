.PHONY: hmk.pdf

default: hmk.sty hmk.pdf

hmk.sty:
	tex hmk.ins

# \GetFileInfo works only when hmk.sty exists
hmk.pdf: hmk.sty
	pdflatex hmk.dtx
	pdflatex hmk.dtx
	makeindex -s gind.ist -o hmk.ind hmk.idx
	makeindex -s gglo.ist -o hmk.gls hmk.glo
	pdflatex hmk.dtx

clean:
	-rm hmk.aux hmk.glo hmk.gls hmk.idx hmk.ilg hmk.ind hmk.log hmk.out hmk.sty hmk.toc 2>/dev/null
