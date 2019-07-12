FILE = $(wildcard *.tex)
PDF  = $(FILE:.tex=.pdf)
AUX  = $(FILE:.tex=.aux)
LOG  = $(FILE:.tex=.log)

.PHONY:run
run:$(PDF)

%.pdf: %.tex
	pdflatex -synctex=1 $<
	# pbibtex $*
	# cmd /c start $@

#クリーンして実行
.PHONY: all
all: clean run

#クリーン
.PHONY:clean
clean: 
	rm -f $(PDF) $(AUX) $(LOG)
