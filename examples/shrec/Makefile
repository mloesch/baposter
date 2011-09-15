ALL: poster.pdf poster_landscape.pdf 

%.pdf: %.tex Makefile
	pdflatex $< &&	pdflatex $< && pdflatex $<

clean:
	  rm -f *.aux	*.bbl	*.blg	*.log	poster.pdf poster_landscape.pdf
