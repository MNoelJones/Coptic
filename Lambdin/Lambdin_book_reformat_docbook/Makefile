all: Lambdin_complete.pdf

%.pdf: %.xml
	pandoc $< -o $@ -f docbook


%_complete.xml: %.xml
	xmllint $< --xinclude > $@


clean:
	rm *_complete.pdf
	rm *_complete.xml