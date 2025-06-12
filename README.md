# COMP-8780-Assignment-4-solution

Download Here: [COMP 8780 Assignment #4 solution](https://jarviscodinghub.com/assignment/comp-8780-assignment-4-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

1. Extract from the BROWN file all grammar rules embedded in parse
trees. Do not consider punctuation as a nonterminal. Eliminate
numbers attached to non-terminals such as ‘-1’, ‘-2’, etc. Report
how many distinct rules you found, what are the 10 most frequent
rules regardless of the non-terminal on the left-hand side, and
what is the non-terminal with the most alternate rules (i.e. the
non-terminal that can have most diverse structures). [20 points]

2. Try to estimate how large the above grammar would be if you were to
lexicalize it, i.e. to add head words to some of the rules. Work
with your own assumptions. The important part for this problem is
your general reasoning and not the details. [20 points]

HINT FOR PROBLEM 1: read one parse tree at a time from the file,
traverse the tree and whenever you visit a node display the grammar
rule associated with the node. To print the grammar rule print the tag
of the node then ‘->’ followed by the tags of children separated by
spaces. Pass the output to the ‘sort’ and ‘uniq’ commands (if in a
UNIX environment).

NOTE: Only consider rules that have a non-terminal on the left hand
side.

—

SAMPLE GRAMMAR RULES EXTRACTED FROM FIRST 3 PARSE TREES IN THE SnapshotBrown.pos.all.txt FILE.

S -> NP VP
NP -> DT NNP NNP NNP NNP
VP -> VBD NP SBAR
SBAR -> S
S -> NP VP
NP -> DT NN PP
VP -> VBD NP
PP -> IN NP
NP -> NP POS JJ JJ NN
NP -> NNP
VP -> VBD NP
NP -> DT NN SBAR
SBAR -> IN S
S -> NP VP
NP -> DT NNS
VP -> VBD NP
NP -> NN

S -> NP ADVP VP
NP -> DT NN
ADVP -> RB
VP -> VBD PP SBAR
PP -> IN NP
NP -> JJ NNS
SBAR -> IN S
S -> NP VP
NP -> NP SBAR
NP -> DT NNP NNP NNP
SBAR -> WHNP S
WHNP -> WDT
S -> NP VP
VP -> VBD NP
NP -> ADJP NN PP
PP -> IN NP
NP -> DT NN
VP -> VBZ NP
NP -> DT NN CC NNS PP PP
PP -> IN NP
NP -> DT NNP PP
PP -> IN NP
NP -> NNP
PP -> IN NP
NP -> NP SBAR
NP -> DT NN
SBAR -> WHPP
WHPP -> IN WHNP
WHNP -> WDT
S -> NP AUX VP
NP -> DT NN
AUX -> VBD
VP -> VBN

S -> NP AUX VP
NP -> DT NNP NN NN
AUX -> VBD
VP -> VBN VP
VP -> VBN PP S
PP -> IN NP
NP -> NNP NNP NNP NNP NP
NP -> NNP NNP
S -> NP AUX VP
VP -> VB NP
NP -> NNS PP
PP -> IN NP
NP -> JJ NNS PP
PP -> IN NP
NP -> NP SBAR
NP -> DT ADJP NN
ADJP -> JJ
SBAR -> WHNP WDT
S -> NP AUX VP
VP -> VBN PP
PP -> IN NP
NP -> NNP NP
NP -> NNP NNP NNP

