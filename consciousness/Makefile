all: consciousness.pdf

%.pdf: %.tex
	latexrun --latex-cmd=xelatex -o $@ $<
	# Compile again (because LaTeX)
	latexrun --latex-cmd=xelatex -o $@ $<

.PHONY: clean

clean:
	rm -rf latex.out
