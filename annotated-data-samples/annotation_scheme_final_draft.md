# Annotation Scheme 

| 1 tag   | Utterance - uttr                          |
| ------- | ------------------------------------------- |
| kz     | Kazakh      |
| rs     | Russian        |


- adding this class helps to later calculate multilingual index, integration index, and L1-L2 ratio within dataset to describe code-switching type: 
- if it is balanced CS; 
- is there a language shift happening; 
- syntactic integration level of code-switching fragments;


| 2 tag           | Code-switching types - cs                |
| --------------- | --------------------------------------------------- |
|**inter-sentential** | 1st utterance in Kaz and 2nd in Rus or vice-versa |
| uttr            | utterance (since this is a spoken data)             |
|**intra-sentential** | within one utterance |
| disc            | discourse marker                                    |
| phr             | phrase (a group of words)                           |
| vp              | verbal phrase, Russian verb+Kazakh verbs+affixes    |
| cl              | clause                                              |
|**intra-word** |words that have an alternative in Kazakh |
| n               | noun                                                |
| adj             | adjective                                           |
| adv             | adverb                                              |
| pn              | pronoun                                             |
| conj            | conjunction                                         |
| interj          | interjection                                        |
| morph           | Russian stem (any POS) with Kazakh affixes          |
| part            | particles                |
| vb              | verbs                 |
| other           | Russian numericals, slang words, etc.               |


### Basic format of code-switching tags:

<uttr lang = ‘kaz’|‘rus’> </uttr>  <br />
<cs = 'inter-sent'|' intra-sent'|'intra-word' <br />
disc = 'discourse marker' <br />
phr = ‘phrase’ <br />
vp = ‘verbal phrase, Russian verb followed by Kazakh modal verbs and affixes’ <br />
cl = ‘clause’ <br />
morph = ‘Russian stem followed by Kazakh affixes’ <br />
pos = ‘n’|’adj’|’adv’|’pn’|’conj’|'interj'| 'vb' > <br />
code-switching instance </cs>  


