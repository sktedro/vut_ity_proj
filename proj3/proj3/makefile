NAME=proj3
LOGIN=xskalo01

ALLFILES=./* ./*/*

DEFAULT: pdf

pdf: $(NAME).tex
	latex $(NAME).tex
	latex $(NAME).tex
	dvips -sPAPERSIZE=a4 $(NAME).dvi
	ps2pdf -sPAPERSIZE=a4 $(NAME).ps

zip: clean
	zip $(LOGIN)-fit.zip $(ALLFILES)

clean:
	rm -f *.aux *.log *.zip *.dvi *.ps *.pdf *.out src/*.pdf
