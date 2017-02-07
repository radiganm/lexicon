#!/usr/bin/make
## makefile (for mandarin)
## Mac Radigan

.PHONY:
.DEFAULT_GOAL := default
SHELL = /bin/zsh
language = mandarin

default: doc

doc:
	cat **/*.md > $(language).cat
	pandoc                                   \
	     --latex-engine=xelatex              \
	 -V mainfont=WenQuanYi\ Micro\ Hei\ Mono \
	        $(language).cat                  \
	     -f markdown                         \
	     -t latex                            \
	     -o $(language).pdf

## *EOF*
