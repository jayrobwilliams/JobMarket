all:	card.pdf card.png clean

card.pdf: card.tex
	lualatex -interaction=nonstopmode card
	
card.png: card.pdf
	convert -background white -density 550 card.pdf -quality 100 -resize 700x400 card.png

clean: 
	rm -vf *.aux *.log