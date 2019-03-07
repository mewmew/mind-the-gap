all: dualism_presentation.pdf

%.pdf: %.tex
	latexrun --latex-cmd=xelatex -o $@ $<
	# Compile again (to fix section progress bar).
	latexrun --latex-cmd=xelatex -o $@ $<

.PHONY: all clean

clean:
	$(RM) -v -rf latex.out
	$(RM) -v dualism_presentation.pdf
