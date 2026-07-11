LATEXMK = latexmk
MAIN = main.tex

.PHONY: all clean distclean

all:
	$(LATEXMK) -xelatex $(MAIN)
	@cp build/$(MAIN:.tex=.pdf) ./

clean:
	$(LATEXMK) -c $(MAIN)

distclean:
	$(LATEXMK) -C $(MAIN)
	rm -rf build

pdf: all
	@echo "PDF generated: $(MAIN:.tex=.pdf)"
