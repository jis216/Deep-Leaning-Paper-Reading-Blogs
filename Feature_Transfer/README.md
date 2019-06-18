# Explore feature transfer in deep neural netowrks

Related paper: [How Transferable are Features in Deep Neural Networks][Paper Link] by Jason Yosinski et al.

It's common to transfer features from a model trained on a large dataset to a small dataset for a similar task. Yet how should we quantify the transferability between datasets and tasks? Which layers of model are "general" enough for us to transfer and which are not? The publication [How Transferable are Features in Deep Neural Networks][Paper Link] composed by Jason Yosinski et al. addressed these questions through the comparison between models of same structure trained on different ImageNet subsets.

### General or Specific?
When we are transfering features between networks trained for different tasks, we always need to consider whether these features are "general" enough for a successful transfer. In other words, we need to define a way to quantify the degree to which a particular layer is general or specific so that we could tell how well features would transfer from one task to another.
 
### Measures Generality as Transfer Performance

<img src="/images/Figure1.png" width="200"/>
Figure 1: Overview of the experimental treatments and controls.

In the paper, Yosinski defines the degree of generality of a set of features learned on task A as the extent to which the features can be used for another task B. To measure this generality, the paper sets up an experiment that compares the performance of models on classification tasks A and B by constructing pairs of non-overlapping subsets of the ImageNet dataset.

Specifically, A and B would each contains 500 classes from the 1000 ImageNet classes. They trained one eight-layer convolutional network on A and another on B, which are named as baseA and baseB correspondingly (reopresented as the top two rows of Figure 1). Then the first n layers (n from 1-7) are transfered from model trained for task A to model trained for task B. To be specific, these networks were named as:

Transferred and frozen layers:
- A *selffer* network BnB: the first n layers are copied from baseB and frozen. 
- A *transfer* network AnB: the first n layers are copied from baseA and frozen.

Transferred and fine-tuned layers:
- A *selffer* network BnB+: the first n layers are copied from baseB and allowed to learn. 
- A *transfer* network AnB+: the first n layers are copied from baseA and allowed to learn.

h<sub>&theta;</sub>(x) = &theta;<sub>o</sub> x + &theta;<sub>1</sub>x

The above process was also repeated in the other direction (task B to A).


The research concluded the negative impact of 
> The overriding design goal for Markdown's
> formatting syntax is to make it as readable
> as possible. The idea is that a



   [Paper Link]: <https://papers.nips.cc/paper/5347-how-transferable-are-features-in-deep-neural-networks.pdf>

