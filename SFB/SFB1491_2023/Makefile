MAIN=poster-template
LATEX=lualatex -interaction=nonstopmode -halt-on-error

# GhostScript prevents errors stemming from the printer firmware
print-$(MAIN).pdf: $(MAIN).pdf
	gs -dNoOutputFonts -sDEVICE=pdfwrite -r600x600 -o $@ $<

# usual LaTeX compilation
$(MAIN).pdf: $(MAIN).tex $(MAIN).bib $(shell find img -type f)
	- $(LATEX) -shell-escape $(MAIN)
	- bibtex $(MAIN)
	- $(LATEX) $(MAIN) > /dev/null
	$(LATEX) $(MAIN)

clean:
	rm -f $(MAIN).pdf print-$(MAIN).pdf \
	  *.aux *.auxlock *.bbl *.blg *.loa *.lof *.log *.out *.thm *.toc

.PHONY: clean
