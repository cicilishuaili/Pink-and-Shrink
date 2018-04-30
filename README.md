# Pink-and-Shrink

## Motivation
Language is powerful, and not only in the ways we use it for communication and expression. Studies have shown that the medium with which we share our thoughts, ideas, beliefs in, inadvertently influences and shapes us. From [national identity](https://www.npr.org/sections/parallels/2017/09/29/554327011/for-catalonias-separatists-language-is-the-key-to-identity), to [our spending habits](http://www.anderson.ucla.edu/faculty/keith.chen/papers/LanguageWorkingPaper.pdf), to perceptions of [time](http://journals.sagepub.com/doi/abs/10.1177/0956797610386621), [agency](https://www.frontiersin.org/articles/10.3389/fpsyg.2010.00162/full), and [art](https://www.frontiersin.org/articles/10.3389/fpsyg.2010.00244/full), the features of language matter more than you may think. As a speaker of two languagages without grammatical gender, I found it especially interesting the way that can affect [how inanimate objects are described](https://web.stanford.edu/class/linguist156/Boroditsky_ea_2003.pdf), showing just how certain ideas, stereotype or not, can be ingrained and propagated via language.

The pervasiveness of the feminine connotation and the ability for that to transfer to objects is also met from the other side, as "Shrink it and pink it" has been the marketing mantra that goes into product design for women. Recalling the infamous Bic's "for her" pens, the assumption has always been that ladies are obvious dainty and love all shades of magenta. This has also translated into economic implications, where gender-specific item pricing implies a surcharge of [7 percent for women](https://www1.nyc.gov/site/dca/partners/gender-pricing-study.page). Beyond the not easily dismissed financial implications, I became curious; how are these male-female versions of products being described? Have we evolved much from the era of pink and shrink? Are we still, consciously through marketing, or unconsciously through masculine and feminine adjectives, transferring something in those words?

Fascinated by the ways description and perceptions are embedded in our lives, I aim to probe at the intersection of objects, language, and gender.

## Story (optional reading)
[Read about it here](https://github.com/cicilishuaili/Pink-and-Shrink/blob/master/Optional_Origin_Story.md)

## Problem
How do product descriptions vary across the gender aisle? Are they a reflection of specilized functional design or an appeal to more stereotypical perception? Can we predict the "gender" of an item, solely based on its descriptions?

## Data Source
There is no online market more ubiquitous than Amazon. The product descriptions can be available via their Amazon Product Advertisement API, requiring an associates account (free). Although it is a bit restrictive in the amount of information that is accessible (e.g. they only allow a search to fetch 10 pages instead of the old 100 back in the days), it will do as initial exploration that can still reveal useful insights. 

Since I am a relatively new to interacting with APIs, I looked for and used one of the more [well documented wrapper for Python](https://python-amazon-product-api.readthedocs.io/en/latest/index.html). It performs adequately and serves its purpose well for now at least. But the big thing I realized a bit late is that its compatibility is limited to Python 2.7 so I may be motivated to change. I recently just found another (perhaps more flexible wrapper)[https://github.com/lionheart/bottlenose], to experiment with in the future should I want to do something like play with the parsing option. I don't foresee the need, unless one feels particularly ambitious, for scraping, especially since amazon's robots.txt seem to be quite restrictive.

## Analysis
The basic plan of approach thus far:

1. Find product categories that are, or should be, essentially functional equivalents in use, regardless of gender.
2. Obtain product descriptions for items that are for women vs. men.
2. Use NLP and other techniques to determine the key differences between the two categories of description. Naive bayes seems like a good place to start given its simplicity and ease of interpretation.

I look forward to learning various useful tools concerning NLP in particular. The project can be extended to other regions, to see if there are differences across the English speaking regions, or if they reinforce patterns. Different languages is a reach but may prove more interesting since many languages have grammatical gender, naturally lending itself to the larger question of not just product design, but inherent perception of items as a certain gender. 

## Deliverables

Easy to interpret graphics that exhibit simple yet profound insights into the world of gendered product descriptions. Once I get more comfortable with basic Flask/Django and Heroku deployment, I would really love to deliver an interactive graphics app to showcase and highlight interesting findings.
