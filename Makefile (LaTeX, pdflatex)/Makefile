FILE = $(wildcard *.tex)
PDF  = $(FILE:.tex=.pdf)

.PHONY:run
run:$(PDF)

%.pdf: %.tex
	pdflatex $<
	# pbibtex $*
	# cmd /c start $@

#クリーンして実行
.PHONY: all
all: clean run

#クリーン
.PHONY:clean
clean: 
	rm -f $(PDF)
