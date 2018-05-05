all :
	mkdir -p out
	pandoc -t revealjs \
		--self-contained \
		-o ./out/presentation.html \
		-V revealjs-url=./reveal.js \
		./src/presentation.md

revealjs :
	wget https://github.com/hakimel/reveal.js/archive/master.tar.gz
	tar -xzvf master.tar.gz
	mv reveal.js-master reveal.js
	rm master.tar.gz

clean :
	rm -rf reveal.js out

.PHONY : all revealjs clean
