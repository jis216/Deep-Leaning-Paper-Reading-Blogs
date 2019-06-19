# Notes on Language Modeling
**Related Resources:**
Michael Collins: [Course Notes for COMS w4705: Language Modeling](http://www.cs.columbia.edu/~mcollins/courses/nlp2011/notes/lm.pdf)

**Keywords:**
- corpus: set of sentences in some language
- 

## What is Language Modeling?
Assume that we have a vocabulary V that is the set of all words in the language. For example, we might have several years of text from the New York Times. Given this corpus, we'd like to estimate the parameters of a language model. And we assume that x<sub>n</sub> is a special symbo STOP. We'll define V<sup>+</sup>  to be the set of all sentences with the vocabulary V: this is an infinite set.

Language Model:
**Definition 1**: A language model consists of a finite set V, and a function *p(x<sub>1</sub>, x<sub>2</sub>, ... x<sub>n</sub>)* such that:
*1. For any <x<sub>1</sub>, ... x<sub>n</sub>> &isin; V<sup>+</sup>, p( x<sub>1</sub>, x<sub>2</sub>, ... x<sub>n</sub> ) = 1*

*2. In addition,*


<!--stackedit_data:
eyJoaXN0b3J5IjpbMTIyOTg5MTg0OSwtNDY5Njg2NzI1LC0xND
gwODU4OTg2LC0yNjEwNjI0N119
-->