# Annotation Scheme 

| 1 class | Lang – language                             |
| ------- | ------------------------------------------- |
| kaz     | Kazakh (for each token ‘automatically’)     |
| ------- | ------------------------------------------- |
| rus     | Russian (manually while annotating)         |


- adding this class helps to later calculate multilingual index, integration index, and L1-L2 ratio within dataset to describe code-switching type: 
-[x]if it is balanced CS; 
-[x]is there a language shift happening; 
-[x]syntactic integration level of code-switching fragments;


| 2 class         | CS_type tags – code-switching types                 |
| --------------- | --------------------------------------------------- |
|inter-sentential (1st utterance in Kaz and 2nd in Rus or vice-versa)   |
| --------------- | --------------------------------------------------- |
| uttr            | utterance (since this is a spoken data)             |
| --------------- | --------------------------------------------------- |
| intra-sentential                                                      |
| --------------- | --------------------------------------------------- |
| disc            | discourse marker                                    |
| phr             | phrase (a group of words)                           |
| vp              | verbal phrase, Russian verb+Kazakh verbs+affixes    |
| cls             | clause                                              |
| --------------- | --------------------------------------------------- |
| intra-word (words that have an alternative in Kazakh)                 |
| --------------- | --------------------------------------------------- |
| n               | noun                                                |
| adj             | adjective                                           |
| adv             | adverb                                              |
| pn              | pronoun                                             |
| conj            | conjunction                                         |
| morph           | Russian stem (any POS) with Kazakh affixes          |





