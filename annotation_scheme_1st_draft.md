# Annotation Scheme 

| 1 tag   | Utterance - uttr                          |
| ------- | ------------------------------------------- |
| kaz     | Kazakh      |
| rus     | Russian        |


- adding this class helps to later calculate multilingual index, integration index, and L1-L2 ratio within dataset to describe code-switching type: 
- if it is balanced CS; 
- is there a language shift happening; 
- syntactic integration level of code-switching fragments;


| 2 tag           | Code-switching types - cs_type                 |
| --------------- | --------------------------------------------------- |
|inter-sentential | 1st utterance in Kaz and 2nd in Rus or vice-versa |
| uttr            | utterance (since this is a spoken data)             |
| intra-sentential | within one utterance |
| disc            | discourse marker                                    |
| phr             | phrase (a group of words)                           |
| vp              | verbal phrase, Russian verb+Kazakh verbs+affixes    |
| cls             | clause                                              |
| intra-word |words that have an alternative in Kazakh |
| n               | noun                                                |
| adj             | adjective                                           |
| adv             | adverb                                              |
| pn              | pronoun                                             |
| conj            | conjunction                                         |
| morph           | Russian stem (any POS) with Kazakh affixes          |


### Basic format of code-switching tags:

<u> lang = ‘kaz’|‘rus’ </u>

<cs cs_type = 'inter-sent'|' intra-sent'|'intra-word' 
disc = 'discourse marker' 
phr = ‘phrase’ 
vp = ‘verbal phrase, Russian verb followed by Kazakh modal verbs and affixes’ 
cls = ‘clause’ 
morph = ‘Russian stem followed by Kazakh affixes’ 
pos = ‘n’|’adj’|’adv’|’pn’|’conj’> 
code-switching instance </cs>



