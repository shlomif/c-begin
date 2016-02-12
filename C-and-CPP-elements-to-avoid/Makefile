DOCBOOK5_XHTML_BASE = as-xhtml
DOCBOOK5_XHTML = $(DOCBOOK5_XHTML_BASE)/index.html
DOCBOOK5_DOC = c-and-cpp-elements-to-avoid.docbook5.xml

all: $(DOCBOOK5_XHTML) $(DOCBOOK5_DOC)

$(DOCBOOK5_DOC): c-and-cpp-elements-to-avoid.xml-grammar-vered.xml
	./bin/translate-Vered-XML --output "$@" "$<"

$(DOCBOOK5_XHTML): $(DOCBOOK5_DOC)
	docmake -v -o $(DOCBOOK5_XHTML_BASE) -x lib/sgml/shlomif-docbook/xsl-5-stylesheets/shlomif-essays-5-xhtml-onechunk.xsl xhtml-1_1 "$<"
