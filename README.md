# Pink-and-Shrink

## Motivation
Language is powerful, and not only in the ways we use it for communication and expression. Studies have shown that the medium with which we share our thoughts, ideas, beliefs in, inadvertently influences and shapes us. From [national identity](https://www.npr.org/sections/parallels/2017/09/29/554327011/for-catalonias-separatists-language-is-the-key-to-identity), to [our spending habits](http://www.anderson.ucla.edu/faculty/keith.chen/papers/LanguageWorkingPaper.pdf), to perceptions of [time](http://journals.sagepub.com/doi/abs/10.1177/0956797610386621), [agency](https://www.frontiersin.org/articles/10.3389/fpsyg.2010.00162/full), and [art](https://www.frontiersin.org/articles/10.3389/fpsyg.2010.00244/full), the features of language matter more than you may think. As a speaker of two languagages without grammatical gender, I found it especially interesting the way that can affect [how inanimate objects are described](https://web.stanford.edu/class/linguist156/Boroditsky_ea_2003.pdf), showing just how stereotypes can be ingrained and propagated via language.

Fascinated by the ways description and perceptions are embedded in our lives, I aim to probe at the intersection of objects, language, and gender.


## Problem
Can we predict the "gender" of an item, solely based on its descriptions?

## Data Source
There is no online market more ubiquitous than Amazon. The product descriptions can be available via their Amazon Product Advertisement API. Although it is a bit restrictive in the amount of information that is easily accessible, it will do as initial exploration that can still reveal useful insights.

## Analysis
The basic plan of approach thus far:

1. Find product categories that are, or should be, essentially functional equivalent in use, regardless of gender.
2. Obtain product descriptions for items that are for women vs. men.
2. Use NLP and other techniques to determine the key differences among the two categories of description. Naive bayes seems like a good place to start given its simplicity and ease of interpretation.

I look forward to learning various useful tools concerning NLP in particular. The project can be extended to other regions/languages if suitable data sources are found, and may prove more interesting since many languages have grammatical gender, naturally lending itself to the larger question of not just product design, but inherent perception of items as a certain gender. 
