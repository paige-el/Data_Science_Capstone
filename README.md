# Building an Instacart Recommendation Engine Data Science Capstone Brief (Read Me File)

## Goals
I am a UX designer by trade and on of the ways I’ve seen users begin interacting with data science concepts in a user interface is through recommendation engines. I’m interested in understanding how these work on the backend so I can better design for them in interfaces and speak to how they work
 
## Problem Statement
BLUF : Traditional grocery stores have better conditions for spontaneous user purchases because every possible purchase item is displayed to the user and they have to physically look through aisles of products for the items on their list. Users that like the novelty of discovering new items in a grocery store may miss the the novelty of finding new items this way when switching to an app. Recommendation engines may be able to help users discover new products and keep that novelty alive.
One of the reasons I haven’t switched over to ordering my groceries on something like Instacart is because of the way I shop and eat. I’m kind of a lazy cook and I’ve gotten super in weightlifting this year so I track my macros and calories (I’m becoming a gym bro against my better judgement). I have a few different varieties of things I’ll make for breakfast, lunch, dinner, snacks that I know I like and that fit my nutrition goals.
This is great except that if I kept to that strictly I’d get bored super easily. So when I grocery shop I always pick up a few fun things to keep some novelty in my diet. And I do this by aimlessly wandering the isles and grabbing things that sound interesting and that I might like. There is so much less joy in life if you don’t make room for discovering mochi ice cream you know?
I don’t think I’m the only person that sticks to a list but gives themselves the flexibility to incorporate a few novel things in to their grocery shop. Building in a recommendation engine to Instacart might help optimize finding new novel items because it would be based off of past purchase history.
 
## Hypothesis
Based on a users purchase history and looking at users similar to them, we can find five items at Instacart given store that a target user may be interested in purchasing.
 
## Assumptions
Recommendations will be more accurate if the user has a more established purchase history. This is because we will have more data on the user to pull from.
 
## Goals and success metrics
The goal is to make a recommendation engine that gives a target user 5 recommended store items. Since I am new to data science and we learned NLP late I am going to consider success if I can actually make a recommendation engine that does that. From there I can suggest ways to optimize it and make it more nuanced in how it pulls recommendations.
 
## Risks or limitations
The Instacart data set is pretty large and unfortunately I have the basic build, lowest memory Mac. So I just did not have enough memory to run the whole data set
   
I ran a smaller subset of the data (the first 25,0000 users). Running the model with the full data set could increase the models usefulness as it would have more user order histories to pull from and make correlations.

## Findings
I was able to make a basic recommendation engine on the Instacart data. I think with some additional factors it could be implemented in to the user interface and tested.
 
The first factor I would look at would be – how to we keep recommendations from not being repetitive? 3 of the 5 recommendations my engine returned were greek yogurt in different flavors. My hypothesis would be that users may prefer more variety in what recommendations they are shown
Depending on where the recommendation engine is placed there are some changes we may want to make so its recommendations are as relevant as possible. Ex: If the recommendation engine is placed at the checkout it may make sense to tailor the model to be based on what the user is currently buying.

## Next Steps
Next I would look at time since order – What if our users shopping habits have changed? What if they decided to go vegetarian? Or on a diet? Or what produce they buy is seasonal? Currently the model looks at everything they’ve ever bought and recommends off of that. I’d like to see the model take change in purchase patterns in to account somehow
Finally I would use the whole data set. My computer could just only handle a subsection of the data. Using all of it would yield more refined results as there would be more user profiles to pull from.


## Final Thoughts
Overall my goal in taking this class was to be able to speak to data science concepts at a high level and I feel I have accomplished that. As a UX designer, I work with both data scientists and the stakeholders that request adding AI/ML to their projects. Being able to translate between my very technical data science counterparts and my stakeholders is going to be a hugely valuable skill.
