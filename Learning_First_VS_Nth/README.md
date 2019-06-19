.markdown-here-wrapper{
}
# Learning the First Thing vs. the N-th Thing

Related paper: [Is Learning the N-th Thing any Easier than Learning the First?][Thrun] by Sebastian Thrun.

One main difference between human learning and neural network learning, is that unlike networks trained for one specific tasks, humans encounter a whole stream of learning problems over their entire lifetime. When humans encounter a new thing to learn, they could easily transfer information and experiences that stem from other related tasks and utilize them to assist their new learning task. 

To realize such kind of knowledge transfer in the learning process of machine, the *lifelong learning framework* is created. In this framework, it is assumed that a learner faces a whole collection of learning problems over its entire lifetime. This framework is based on the belief that when facing the n-th learning task, a learner can re-use knowledge gathered in its previous n-1 learning tasks to boost the generalization accuracy.

In this paper, Thrun let the learner face a family of *concept learning tasks*. More specifically, the functions to be learned over the liftime of the learner, denoted by *&fnof;<sub>1</sub>, &fnof;<sub>2</sub>, &fnof;<sub>3</sub> &isin; F*, are all of the type functions that defines a particular concept: a pattern *&fnof; : I &rarr;* {0, 1} and sampled from *F*. These functions are indicator functions that each defines a particular concept: a pattern *x &isin; I* is member of this concept iff *f(x)* = 1. When learning the n-th indicator function 


[Thrun]: <https://papers.nips.cc/paper/1034-is-learning-the-n-th-thing-any-easier-than-learning-the-first.pdf](https://papers.nips.cc/paper/1034-is-learning-the-n-th-thing-any-easier-than-learning-the-first.pdf)>
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTQ3NjU2ODUzOSwxNzY3OTY0Nzk2LC0xMj
UzMzgxMDU5LC0xNTA5MjI1NjI1LDE4MzQ4NTYzODldfQ==
-->