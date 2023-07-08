# Haiku-Shakespeare-Generator

## Inspiration For The Project 

This project was created for a class that wanted us students to generate poems in a similar
manner to how word suggestion works when you text! We were provided some helper functions to work 
with but ultimately had to decide what kinda poems we wanted our generator to create and how we went
about generating each line. 

I decided to create a Haiku generator as I thought Haiku's were both simplistic but beautiful to read
and I was really interested to see how it would create lines with few syllables.   

A Haiku is a poem that consists of three lines, with five syllables in the first line, seven in the second, and five in the third. 

I decided to use the Shakespeare corpus as who doesn't want to see poetry in a language that's a bit older?

Additionally, when I was using other corpora, I noticed that some choice words that shouldn't be used were
included. So that led me to only use the Shakespeare corpus.

However, feel free to combine corpora or use any other corpora available in the nltk library! 

## Thoughts and Lessons 

To preface, this project was made when I was learning the basics of Python, so the code may not be written in 
the most optimized way or it may not have taken advantage of as many libraries as it could've. 

However, I do remember learning a lot from such a project in regard to being careful with the outputs and 
inputs of functions as well as debugging as I ran into two massive problems: 

When creating rhyming lines, some words wouldn't have a rhyme so I had to make sure the program randomly selected
a new word that did have words that rhymed with it. Since I didn't know much about testing at the time, it took me 
a while to figure this out as from my perspective, the program would work most of the time but then didn't work 
on rare occasions. This is when I ended up printing line after line of inputs and outputs, leading me to discover 
this problem and fix the function.   

When creating lines with syllable restrictions, I initially hadn't accounted for words with zero syllables or  
if the syllable count was greater than the syllables that were left to be allotted. Without accounting for these two cases 
the generated haikus did not always follow the standard 5/7/5 syllable rule. To resolve this issue, we essentially changed
our code to ignore these cases and to pick another word instead that would fit into our restrictions. 

## Conclusion
Overall, it was a fun project to work on and I'm happy with the final product! 

If there was something that I could improve, it would probably be the algorithm for the word choice 
as the poems do feel a bit awkwardly generated. In the future, I may consider redoing/revamping this 
project with an LLM instead and see how the results pan out. 

