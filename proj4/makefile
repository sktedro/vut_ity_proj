NAME=proj4
LOGIN=xskalo01

ALLFILES=./* ./*/*

DEFAULT: pdf

pdf: $(NAME).tex
	latex --interaction=batchmode $(NAME).tex
	latex $(NAME).tex
	dvips -sPAPERSIZE=a4 $(NAME).dvi
	ps2pdf -sPAPERSIZE=a4 $(NAME).ps
	pdftk ../$(NAME).pdf multibackground $(NAME).pdf output ../overlay.pdf

zip: clean
	zip $(LOGIN)-fit.zip $(ALLFILES)

clean:
	rm -f *.aux *.log *.zip *.dvi *.ps *.pdf *.out src/*.pdf
