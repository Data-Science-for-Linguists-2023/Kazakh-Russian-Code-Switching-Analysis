# Annotation Scheme 

##### 1 class: Lang – language

kaz  - Kazakh (for each token ‘automatically’)
rus – Russian (for each token manually while annotating)

- adding this class helps to later calculate multilingual index, integration index, and L1-L2 ratio within dataset to describe code-switching type: 
-[•]if it is balanced CS; 
-[•]is there a language shift happening; 
-[•]syntactic integration level of code-switching fragments;


##### 2 class: CS_type tags – code-switching types 
(only Russian tokens/chunks/phrases are annotated with this tags)

inter-sentential (1st utterance in Kaz and 2nd in Rus):

- uttr = utterance (since this is a spoken data; so far have not been observed)

intra-sentential:

- disc -  discourse marker
- [•] a word or phrase that is used for organizing discourse: for example, well, so, or in fact
- [•] в общем – in general, all in all;

- phr = phrase (a group of words)
-[•] чисто гипотетически - theoretically  

- vp – verbal phrase, Russian verb + Kazakh modal verbs+affixes, eg.:
-[•] [поздравить еткен жоқпын] - Russian verb+Kazakh modal verb+Kazakh word for ‘no’+1st personal ending


- cls = clause 
-[•] a group of words containing a subject and predicate and functioning as a member of a complex or compound sentence

intra-word
(words that have an alternative in Kazakh but a speaker chooses to use a Russian version):

- n -  noun 
- adj -  adjective 
- adv – adverb
- pn – pronoun 
-[•] что-то - Russian pronoun

- conj -  conjunction 
-[•] a word used to connect clauses or sentences or to coordinate words in the same clause (e.g. and, but, if ).

- morph - Russian stem (any POS) with Kazakh affixes
-[•] cвязін: Russian stem, Noun+Kazakh suffix: (personal ending) + (accusative)
-[•] звондау: Russian stem, Verb+Kazakh verb suffix: да (converts nouns to verbs)+ у (infinitive)
	


