#
# File:   lecturenotes.mak
# Author: Adam Lewis
# Purpose:
# Build lectures notes for a single module
#
# Tools for building latex
LATEXMK = latexmk -f
NBCONV = jupyter nbconvert --to pdf 
RM = rm -f
.PHONY: all mostlyclean clean release part1 part2

# Rules
%.pdf: %.ipynb
	$(NBCONV) $*

# Targets
MODNAME1=Module00PartA
MODNAME2=Module00PartB
MODNAME3=Module00PartC
MODNAME4=Module00PartD
# MODNAME5=Module00PartE
# MODNAME6=Module00PartF
# MODNAME7=Module00PartG
# MODNAME8=Module00PartH
# MODNAME9=Module00PartI
# MODNAME10=Module00PartJ
# MODNAME11=Module00PartK

#all: part1 part2 part3
all: part1

part1: $(MODNAME1) $(MODNAME2) $(MODNAME3) $(MODNAME4) $(MODNAME5)

part2: $(MODNAME6) $(MODNAME7) $(MODNAME8) $(MODNAME9)

part3: $(MODNAME10) $(MODNAME11)

release: all mostlyclean

$(MODNAME1): $(MODNAME1).pdf 

$(MODNAME1).pdf:  $(MODNAME1).ipynb

$(MODNAME2): $(MODNAME2).pdf

$(MODNAME2).pdf:  $(MODNAME2).ipynb

$(MODNAME3): $(MODNAME3).pdf 

$(MODNAME3).pdf:  $(MODNAME3).ipynb

$(MODNAME4): $(MODNAME4).pdf

$(MODNAME4).pdf:  $(MODNAME4).ipynb

$(MODNAME5): $(MODNAME5).pdf

$(MODNAME5).pdf:  $(MODNAME5).ipynb

$(MODNAME6): $(MODNAME6).pdf

$(MODNAME6).pdf:  $(MODNAME6).ipynb

$(MODNAME7): $(MODNAME7).pdf

$(MODNAME7).pdf:  $(MODNAME7).ipynb

$(MODNAME8): $(MODNAME8).pdf

$(MODNAME8).pdf:  $(MODNAME8).ipynb

$(MODNAME9): $(MODNAME9).pdf

$(MODNAME9).pdf:  $(MODNAME9).ipynb

$(MODNAME10): $(MODNAME10).pdf

$(MODNAME10).pdf:  $(MODNAME10).ipynb

$(MODNAME11): $(MODNAME11).pdf

$(MODNAME11).pdf:  $(MODNAME11).ipynb


# Clean targets

clean: 
	$(RM) *.pdf
