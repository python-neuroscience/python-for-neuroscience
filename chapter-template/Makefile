SOURCES  = $(wildcard *.md)
OBJECTS  = $(SOURCES:.md=.pdf)
BIBFILE  = chapter.bib
BIBSTYLE = frontiers.csl
FORMAT   = markdown+simple_tables+table_captions+mmd_title_block+fenced_code_attributes

all: $(OBJECTS)

%.pdf: %.md %.bib Makefile template.latex
	@printf "Processing $< ... "
	@pandoc --smart --standalone --from $(FORMAT)       \
                --latex-engine=pdflatex                     \
                --filter pandoc-citeproc                    \
                --highlight-style=tango                     \
                --variable fontsize=10pt                    \
                --variable urlcolor=blue                    \
                --variable citecolor=blue                   \
		--variable mainfont="MinionPro-Regular"     \
		--variable monofont="Source Code Pro Light" \
                --latex-engine=xelatex                      \
                --template template.latex                   \
                --csl=$(BIBSTYLE)                           \
                --bibliography=$(BIBFILE) -o $@ $<
	@printf "done.\n"


clean:
	rm -f $(OBJECTS)
