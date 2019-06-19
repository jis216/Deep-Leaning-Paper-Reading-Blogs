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
*1. For any <x<sub>1</sub>, ... x<sub>n</sub>> &isin; V<sup>+</sup>, p(x<sup>1</sup>, x<sup>2</sup>, ... x<sup>n</sup>)*
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE0NDg3ODgwNTAsLTQ2OTY4NjcyNSwtMT
Q4MDg1ODk4NiwtMjYxMDYyNDddfQ==
-->