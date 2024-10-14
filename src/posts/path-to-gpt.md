---
title: Path to GPT
bibliography: ../zotero.bib
---

*Last updated*: Oct 11, 2024.
---

This post is my attempt to draw the shortest path from knowing a little bit of ML
to understanding state of the art language models (GPTx). It includes both milestone
papers and the best resources I've found to understand a concept. I also like knowing 
the history of things so there will be a bunch of papers that might really
only be of historical interest.

This is a _personal_ path, with the goal of being a reasonably
good practitioner of ML, not a researcher. Finally, "path" is a misnomer. It's
more like a garden to get lost in.

## Math background

There is no end to the amount of math one _could_ learn before studying ML, and
usually the more I learn the more it seems to help. However, I've also found that
it's ok to "lazy-load" the required math once you've acquired a decent intuition
in each of the major areas. This section therefore is just going to be a list of
the areas of math that can be helpful and the best resources I've found for learning
them.

**Probability**

Probability is the foundation for all of ML, statistics, and science. It's also _way more_
complicated than our brief encounter with it in high school or college makes us believe. I'm
always on the look out for books and articles that help in developing a good intuition
for probability.

@hamming is one such book.

**Information Theory**

Information seems like the most natural concept to try to understand ML and stats.
Many of the questions of interest can be posed as information theory questions:
"what has a model learnt?", or "what did this experiment tell us?",
"how much can a model of a certain size learn?"

**Linear Algebra**

Linear Algebra has the worst branding in all of math. It's more exciting
to think of the subject as "thinking in high-dimensional spaces". Everything in ML
deals with vectors with impossibly high dimensions (for example, each token in GPT3
is represented as a vector in a ~50,000 dimension space).

The video series "Essence of Linear Algebra" (@3blue1brown) was the
first time linear algebra made any intuitive sense to me.

## Optimization in ML

The goal of all ML training is to find an acceptably low value of the loss function.

## Automatic Differentiation

AD is the key to training large neural networks. AD libraries automatically
figure out the gradient of the loss function as long as the computation of the loss
function is expressed in a form that the library expects. For example, in PyTorch
the computation is expressed as tensor operations.

@baydin_automatic_2015 is a great survey of the various AD methods. For ML training
we care about "reverse mode".

@paszke_pytorch_2019 describes PyTorch, the most widely used library for deep learning
in production.

## What are neural networks?

Neural networks began as the single-layer "perceptron". I think it's important to recognize
the 

Rosenblatt perceptron
Rumelhart backprop

@lecun_backpropagation_1989 did handwriting recognition.

@andrej_karpathy_deep_2022 re-implements that paper with today's hardware.

@krizhevsky_imagenet_2012 kick-started the modern deep learning revolution by achieving
a significant jump in performance on the image recognition task.

## What is language modeling?

## How is language modeling done with neural networks?

Yoshua Bengio - neural language model
unreasonably effectiveness of RNNs

## How to build GPT?

blah

The bitter lesson.

