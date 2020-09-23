### Foundational testing activties

Updated: {docsify-updated}

1. ***Clarify***

It's next to impossible to know every single model of (development/CI/business domain) because for projects that are more complex than trivial it takes a  full competent specialist to maintain the topic - just one tester won't be enough(or you should find another/more rich and deep job, that will take note thsn your pair of attentive eyes) . 

But there's always be the work of making the models of business domain/CI/etc explicit - or in another words making sure everyone understands model the same way but writing/drawing it down. 

Next task would be questioning that model on the reality check ("how does reality accords to that model?") 

2. ***Doubt the existing/explicitly stated model***

Here you already have some picture of how things should work. Now you're, using your experience/skill/techniques, going to walk through that model with magnifier and ask (yourself/everyone that matters/knows) ***" Is that true? "***

*** "Is that true" *** with different meanings
- is this model correct? (In the realm of concept) 
- is this model the way it should be? 
- is reality corresponds with that model? ( something in reality objects or will/should object that model) 


3. ***Solidify assumptions***
Some parts are to be true always. And it's better to make sure they behave the same way always. 

It's better to solidify that assumptions with automation, or, at least, with regular checking

Make sure, automation works on there right level of automation hierarchy and assumptions are straight-forward and unambiguous. 


4.  ***Let people know about your findings***

If your information didn't find the right ears and didn't change the behavior - it's useless. Make sure, that the people that matter will listen to your investigation results. Slightly unsofisticated template (subject to change) of testing report:

1. List of created tickets (with their own template) 
2. Concerns about
- what hadn't been tested properly
- unclear assumptions
- hard/inconvenient process of testing
- inconvenient/prone to errors process of setting application under the test
- any assumptions/insights about, what will make life easier/more maintainable in the long run (more testability / suggesting to change/challenge the current processes/etc) 
3 time spent
4 ( anything else / add your own) 

5. ***Honing your craft*** - learning how to make things more effective

That's basically all the actions  of tester I can draw  off the top of my head.