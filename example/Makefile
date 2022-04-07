

all: page.pdf


DOC_TEMPLATE=template.tex


%.pdf: %.md $(DOC_TEMPLATE)
	@echo "Generating documentation"
	pandoc --template $(DOC_TEMPLATE) $< -o $@


