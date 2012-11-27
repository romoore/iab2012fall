paper:
	latex gnrs 
	-bibtex --min-crossrefs=20 gnrs
	latex gnrs 
	latex gnrs
	dvips -t letter -o gnrs.ps gnrs

pdf: gnrs 
	ps2pdf gnrs.ps

html:	
	latex2html -nonavigation -math -html_version '4.0' -split 0 gnrs.tex

clean:
	rm -f *.dvi *.aux *.bbl *.ps *.pdf *.rtf *.blg *.log *~
