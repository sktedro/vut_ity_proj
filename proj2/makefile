NAME=proj2
LOGIN=xskalo01

ALLFILES=$(NAME).tex makefile

ALL: $(NAME).tex
	latex $(NAME).tex
	latex $(NAME).tex
	pdflatex $(NAME).tex
	pdflatex $(NAME).tex

zip:
	zip $(LOGIN)-fit.zip $(ALLFILES)

clean:
	rm -f $(NAME).log $(NAME).dvi $(NAME).pdf $(NAME).aux $(NAME).out texput.log $(LOGIN)-fit.zip
