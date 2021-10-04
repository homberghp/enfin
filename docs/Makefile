

all: index.html


%.html: %.adoc
	asciidoctorj \
             -b revealjs -a linkcss -a stylesheet=css/asciidoctor.css \
             -a revealjsdir=https://cdn.jsdelivr.net/npm/reveal.js@3.9.2 \
             $<

index.html: index.adoc css/*.css # hardproblems.adoc rules.adoc teaching.adoc badpractices.adoc

clean:
	rm -f index.html
