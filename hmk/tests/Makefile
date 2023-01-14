tests:
	[[ -d out ]] || mkdir out
	for f in src/*.tex; do \
	    pdflatex -output-directory out "$$f" || exit $$?; \
	done

clean:
	-rm -r out
