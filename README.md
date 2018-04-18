# Pink-and-Shrink

## Motivation
Language is powerful, and not only in the ways we use it for communication and expression. Studies have shown that the medium with which we share our thoughts, ideas, beliefs in, inadvertently influences and shapes us. From [national identity](https://www.npr.org/sections/parallels/2017/09/29/554327011/for-catalonias-separatists-language-is-the-key-to-identity), to [our spending habits](http://www.anderson.ucla.edu/faculty/keith.chen/papers/LanguageWorkingPaper.pdf), to perceptions of [time](http://journals.sagepub.com/doi/abs/10.1177/0956797610386621), [agency](https://www.frontiersin.org/articles/10.3389/fpsyg.2010.00162/full), and [art](https://www.frontiersin.org/articles/10.3389/fpsyg.2010.00244/full), the features of language matter more than you may think. As a speaker of two languagages without grammatical gender, I found it especially interesting the way that can affect [how inanimate objects are described](https://web.stanford.edu/class/linguist156/Boroditsky_ea_2003.pdf), showing just how certain ideas, stereotype or not, can be ingrained and propagated via language.

The pervasiveness of the feminine connotation and the ability for that to transfer to objects is also met from the other side, as "Shrink it and pink it" has been the marketing mantra that goes into product design for women. Recalling the infamous Bic's "for her" pens, the assumption has always been that ladies are obvious dainty and love all shades of magenta. This has also translated into economic implications, where gender-specific item pricing implies a surcharge of [7 percent for women] (http://www1.nyc.gov/site/dca/partners/gender-pricing-study.page). Beyond the not easily dismissed financial implications, I became curious; how are these male-female versions of products being described? Have we evolved much from the era of pink and shrink? Are we still, consciously, or unconsciously, transferring something in those words?

Fascinated by the ways description and perceptions are embedded in our lives, I aim to probe at the intersection of objects, language, and gender.

## Story
There has been a series of arrows that directed me to this place.

I have spent months and months trying to formulate an interesting question that can be answered, at least to some extent, with data I can obtain on a scale I can manage. Through one of the many podcasts I listen to, I stumbled upon the study aforementioned concern how objects are described in languages with grammatical gender. Something about it lingered. I was sure I wanted to do something related to the topic of technology and gender. As a high schooler I once delved into the question of why there weren't more women in the STEM fields as part of a spanning senior project. It only seemed appropriate enough now, with my having gone through the engineering education that seems to be pushing progress only to end up amongst almost all exclusive male colleagues, wishing I were a software engineerer having to deal with this problem instead.

With this as my filter, I started to see some potential. My first idea that did not pan through had involved the voice of the online dictionaries. Maybe, I had thought, that there would be a pattern to which voice said which words. It seems like a stretch, but it was at least one I can investigate. After learning to scrape mp3 files, extracting audio features, and trying some machine learning algorithms to classify the voice gender, I felt like I had reached the end of the data. If there were any pattern, I certainly wouldn't have been able to find it.

Then the second serendipity came from a radio interview show I happen to have listened to one very early Sunday morning on a drive to the marathon I signed up to run the day before. The phrase "Pink and Shrink" came up in terms of making products for women. The precise context of the interview has been lost on me since, perhaps it was outdoor equipment, but I definitely started to notice. At around the same time, I started to look into a particular outdoor gear: a backpack for backpacking. 

For more context to this next part, I've always been the frugal one. After realizing that sizing sometimes is the only thing that differs significantly for something like say, t-shirts for men and women, I shop now across all the traditionally mutually exclusive sections of "men", "women", "children". I own quite a few things that are "men" or "kid" sized now, fitting the same and priced or marked down more significantly than their female/adult counterparts. I remember reading something quite a long time ago that explained the cost as more colors and style options having gone into the design for women.

So for a backpack, I did the same. I stared hard and tried to pick up on the differences. Yes, sure, there are slight and various ways in which the pack was designed especially for women, from the dimensions to other details not captured by the descriptions (apparently, women’s backpacks today have more anatomically suitable hip belts). But what stood out to me more than anything were the names. Atmos for men, Aura for women. Ok, I thought, sure, names are names and have gender. And then I saw the colors: “Gamma Red”, “Challenger Blue”, “Vestal Grey” for women, “Rigby Red”, “Unity Blue”, “Abyss Grey” for men. I had to look up what Vestal means. Is it really necessary to prescribe another descriptor to colors? I can assure you that the colors are the same indistinguishable shade of red, blue, and grey. It felt like an extremely unnecessary aspect to segregate on.

From there I just started thinking; what other products that has a gender divide but are essentially the same? 
Deodorant
Shampoo
Glasses
Razors 
T-shirt
Running Shoes
Socks?
Oral care?

On Amazon at first glance, there’s only clothes and toys that are obviously segregated by men and women. But then there’s men’s grooming as a subcategories. And then upon further clicking, you will find that it is "perfume" for her, "cologne" for him. And so I dug in!


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
