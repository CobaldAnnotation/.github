# CoBaLD Annotation Project

<a href="https://creativecommons.org/licenses/by-nc/4.0/"><img src="https://img.shields.io/static/v1?label=license&message=CC-BY-NC-4.0&color=green"/></a>

This is the CoBaLD Annotation Project Github page. Here we present the linguistic annotation standard and publish datasets annotated according to it.

CobaLD Annotation includes morphological, syntactic and semantic markup. The morphosyntax level relies on the UD markup (ссылка), the semantic pattern is based on the Compreno markup (ссылка). Namely, CoBaLD Annotation is a kind of the UD markup enriched with the semantical pattern which, in turn, includes the annotation of word  meanings and the annotation of the relations between words.

# Annotation of word meanings

In Compreno, word meanings are presented in the form of a semantical hierarchy - a tree of a thesaurus type. Its nodes correspond to semantic classes (SCs) -  semantic fields denoting words meanings. The SCs are universal for all languages. Each SC is filled with contents in concrete languages (English, Russian, German, Japanese, and some others) - lexical classes (LCs). 
Total number of the SCs in Compreno is more than 200,000, which seems too much for the machine learning on the corpora of the volume we currently have. Therefore, we decided to reduce the number of classes and use not the full hierarchy but the hierarchy of the hyperonym classes. Namely, we point out not the SCs like GIRL, TEACHER, or RIVAL, but the SC HUMAN instead of them; not the classes TO_RUN, TO_SWIM, TO_JUMP, but the SC MOTION instead, and so on. The hyperonym hierarchy includes about 650 SCs.

The semantic hierarchy of the hyperonym classes is available at the Compreno Semantics Github2 ССЫЛКА.

# Annotation of the relations between words

The semantic links between words in Compreno are expressed through so called deep (semantic) slots (DS) - semantic roles, which correspond to actant valencies (Agent, Object,
Experiencer, Addressee, etc.), adjuncts (Locative, Distance, Time, Condition, Concession, and so on), characteristics (evaluation, colour, weight, speed, price, form, or size), specifications, parentheticals, and others. It gives the opportunity to define all semantic relations for each word, both actant and circumstantial, which provides full markup of all possible semantic dependencies.
However, the description seems too detailed for most purposes as it suggests more than 330 SSs.
Therefore, we decided to reduce the number of categories as well.  

//
в работе
we have reduced the number of
the SSs. For example, full Compreno markup suggests different roles for different characteristic dependencies, such as form, taste, sound, appearance, importance, genuineness, and so on - more than 60
characteristics in total. In the generalized variant, all such characteristics correspond to one characteristical slot. Or, full model contains several Instrument slots, which differ by the SCs each slot can include
(see fig.1) - in the simplified variant, they are joined in one Instrument slot.
Figure 1: Instrument slots in full and in reduced Compreno markup
As a result, the number of hyperonym SCs used in the markup was reduced to ~680 classes, and the
number of the SSs - to 143 slots.

The list and the description of the semantic roles are also available on ССЫЛКА.
These simplified SCs and SSs are used in the final version of the markup in the UD format.

More than that, we reduced the number of the semantic roles. For example, full ABBYY Compreno markup suggests different roles for different characteristic dependencies (that is, weight, speed, size, and so on). In the generalized variant, all such characteristics correspond to one characteristical role. Or, the Compreno model has several slots for temporal relations: Time (‘вчера – yesterday, через два дня – in two days’), Time_Situation (‘когда все приедут – when everybody comes’), Time_Being (‘при Иване Грозном – in times of Ivan the Terrible’). In the generalized presentation, all these roles correspond to only one Time slot.

As a result, the number of the hyperonym semantic classes used in the markup was reduced to about 650 classes, and the number of the semantic roles – to 143 slots.
//

# CoBaLD Annotated Corpora

Currently, 2 corpora annotated according to the given standard are available:

(1) Russian news corpus: it includes more than 400 000 tokens and has the morphosyntax of the 'basic' UD model.
The corpus page is ССЫЛКА. Here a more detailed description of the corpus and the dataset itself are available.

(2) English news corpus: it includes more than 150 000 tokens and has the morphosyntax of the Enhanced UD model.
The corpus page is ССЫЛКА. Here a more detailed description of the corpus and the dataset itself are available.

