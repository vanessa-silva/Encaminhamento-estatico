DOC=report.pdf

all: $(DOC)
	@

%.pdf : %.tex *.tex
	@pdflatex $<
#	@bibtex report.aux
	@pdflatex $< >/dev/null 2>&1
	@pdflatex $< >/dev/null 2>&1
	@make nice

nice :
	rm -fr *.out *.toc *.aux *.log auto *~

clean :
	@make nice
	rm -f $(DOC)
