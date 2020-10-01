### Test the sorting algorithm

What questions will pop up in your mind if you got that task? What can go wrong?

1. Do we really need the sorting algorithm, and not the Apple to banana transmutation? 
2. Do we have enough time for sorting? Maybe we'll only make the first K items sorted? 
3. Are items really sortable, or they just random concepts like chaos, aircraft and morning breakfast (if sortable, what's the comparator?) 
4. What's the inputs? Are they really really big/small? Do they accessible one by one, or all at the same time?or else? Do they change/will change on a process? How do we get them on  the first place? 
5. What resources do we have? 
6. How people want to use the results? 
7. Do we have multiple users? Simultaneously? 
8. Do we have to sort on our resources or clients? 
9. Won't resources be overwhelmed by load? 
10. If there's multiple users, do they
need to keep their sorted items by themselves or should it be public? 
11. Should they pay for that? 
12. What's the risks of errors on 1,2,Nth place?
13. What would be our testing inputs cases? Search space is infinite [0,1,few,lots,ops?]
14. Do we have to preserve an index of equal items? (They can be equal by comparison, but not entirely the same)
15. Is comparison operation always computable? In reasonable amounts of time?
16. What should we do in case of sudden interruption? Should we allow pausing, should we start over?
17. Should we know about ongoing progress like in percent?

----


What other points might concern you, while testing the simple algorithm? :)