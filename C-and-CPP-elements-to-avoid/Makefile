DOCBOOK5_DOC = c-and-cpp-elements-to-avoid.docbook5.xml

all: $(DOCBOOK5_DOC)

$(DOCBOOK5_DOC): c-and-cpp-elements-to-avoid.xml-grammar-vered.xml
	./bin/translate-Vered-XML --output "$@" "$<"
