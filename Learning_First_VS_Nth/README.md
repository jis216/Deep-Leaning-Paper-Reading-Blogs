.markdown-here-wrapper{
}
# Learning the First Thing vs. the N-th Thing

Related paper: [Is Learning the N-th Thing any Easier than Learning the First?][Thrun] by Sebastian Thrun.

One main difference between human learning and neural network learning, is that unlike networks trained for one specific tasks, humans encounter a whole stream of learning problems over their entire lifetime. When humans encounter a new thing to learn, they could easily transfer information and experiences that stem from other related tasks and utilize them to assist their new learning task. 

To simulate such kind of knowledge transfer in the learning process of machine, the *lifelong learning framework* is created. In this framework, it is assumed that a learner faces a whole collection of learning problems over its entire lifetime. This framework is based on the belief that when facing the n-th learning task, a learner can re-use knowledge gathered in its previous n-1 learning tasks to boost the generalization accuracy.

In this paper, Thrun let the learner face a family of *concept learning tasks*. More specifically, there are n concepts to be learned and these concepts are represented by n functions *&fnof;<sub>1</sub>, &fnof;<sub>2</sub>, &fnof;<sub>3</sub> &isin; F*: a pattern *x &isin; I* is member of this concept iff *f(x)* = 1. And if x is not a member, *f(x)* = 0. When learning each function, the learner will be given not only the corresponding training set *X*, but also the other n-1 sets of data for other concept functions. Each additional datatset *X<sub>k</sub>* is called a support set for the training set *X*.

The support sets usually cannot be used directly as training patterns when learning a new concept, since they describe concepts different from the one to be learned. However, some invariant features of the domain could be learned and transferred to new learning tasks and hence improve generalization.

In this paper, Thrun compares several networks that extend the conventional memory-based neural networks with more traditional learning algorithms. Through this comparison, the research wants to demonstrate that, independent of a particular learning approach, more complex functions can be learned from less training data if learning is embedded into a lifelong context. 

## Memory-Based Learning Approaches
Memory-based algorithms memorize all training examples explicitly and interpolate them at query-time. In the paper, it demonstrates three memory-based algorithms and 



[Thrun]: <https://papers.nips.cc/paper/1034-is-learning-the-n-th-thing-any-easier-than-learning-the-first.pdf](https://papers.nips.cc/paper/1034-is-learning-the-n-th-thing-any-easier-than-learning-the-first.pdf)>
<!--stackedit_data:
eyJoaXN0b3J5IjpbNjQ2MjYwNTU0XX0=
-->