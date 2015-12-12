# Importation des variables
include makevars

all: sp cleanrep cleansousrep

# Génération du pdf
sp:	
	TEXINPUTS=${TEXINPUTS}:$(CLSPATH):$(VOCPATH):$(THEMEPATH);\
	export TEXINPUTS;\
	pdflatex $(NOM_FICHIER).tex;\
	pdflatex $(NOM_FICHIER).tex;\
	mv $(NOM_FICHIER).pdf pdf/$(NOM_FICHIER).pdf;\

# Compression du pdf
compress :
	gs -dBATCH -dNOPAUSE -q -sDEVICE=pdfwrite -sOutputFile=pdf/$(NOM_FICHIER)-temp.pdf pdf/$(NOM_FICHIER).pdf
	mv pdf/$(NOM_FICHIER)-temp.pdf pdf/$(NOM_FICHIER).pdf

# Nettoyage total
clean: cleanpdf cleanrep cleansousrep

# Nettoyage du répertoire
cleanrep:	
	rm -f *.aux *.cb *.cb2 *.log *.toc *.out *.snm *.nav

# Nettoyage du sous répertoire
cleansousrep:	
	rm -f sources/*.aux sources/*.cb sources/*.cb2 sources/*.log sources/*.toc sources/*.out sources/*.snm sources/*.nav

# Nettoyage des pdf
cleanpdf:	
	rm -rf pdf/*.pdf
