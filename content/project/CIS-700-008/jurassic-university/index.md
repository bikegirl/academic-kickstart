<img src="../media/shield-only-RGB-4k.png" align="left" width="60" hieght="60"> 
<img src="https://github.com/bikegirl/academic-kickstart/content/project/CIS-700-008/jurassic-university/icon.png" align="right" />

# Introduction: Murder Mystery: Detective Text Adventure Game

HW2 was a collaboration between Michael Shur and Rebecca Iglesias-Flores.  For part 2, we improved the parser inside action_castle.ipynb.  For part 3, it was a tough choice between between Mike's Detective custom game and Becca's Jurassic University custom game, but in the end we decided to go with Mike's Detective custom game.

> `My custom text adventure game is a humorous murder mystery game. It takes place at my fictional version of UPenn and the characters in the game are myself, some classmates, some faculty. I essentially modeled it after the famous game, Clue. "Mr.Body", completely original name, has been killed! Your goal is to find out how he died  and tell the police so you can get back to studying! I chose this topic because out of all the ideas I had (zombie apocalypse, medieval times, etc.), I believe this one will capture and hold the attention of my target audience (i.e. students and faculty at UPenn) the most. As my high school English teacher once said, "What is everyone interested in? THEMSELVES of course!" :)`

## Files submitted:

(there are other files we uploaded into our repo - for our own purposes, but these are definitely in here and titled correctly for grading.)

- word-sense-annotations.json (annotation for action castle)
- action_castle_improved.ipynb
- my_game_improved.ipynb
- playthrough.txt
- README.md

# Part 2: Improve your Parser with Word Embeddings 

We improved the parser using wordnet and word2vec word embeddings.  Our logic was to 1) Generate all combinations of sentences using wordnet, provided by the enumerate_alternatives() method in the skeleton file, then 2) If the user_command did not match any of the enumerated alternatives in the first step, query word2vec using their similarity() method to ensure it reaches a certain threshold (we tested several sentences and found that a threshold of 0.5 would encapsulated most similar sentences the best).  We had an internal dictionary of synonyms (word-sense-annotations.json) that was used to query all the synonyms needed to generate all the alternative sentences in the enumerate_alternatives() method.

# Part 3: Added Sentiment Analysis

To improve the game play experience of our text adventure we leveraged The TextBlob library for sentiment analysis.  In the end, we require the user to enter two negative sentiment insults in order to leave the basement stairs and win the game.  A few examples are 1) Yo mamma is so ugly when she tried to join an ugly contest they said, "Sorry, no professionals." and 2)
Your feet smell; I hate you!, which is demonstrated in our playthrough.txt.  Feel free to experiment with all sorts of insults to Becca when you play the game.

## Things to acquire in order to complete the game

1. `flashlight`

2. `key`

3. `academic journal`


## How do you win
- Find the person that killed Mr. Body
- Make sure you look and examine everything, because the clues will let you know when you need to talk to someone and their responses might change depending what is in your inventory or where you are.  So even though you've already "talk to Michael," if the adventure game tells you to talk to Michael again, you might want to do it... his script might have changed! 

[Run the Jurassic University Colab]
[Run the Murder Mystery Text Adventure Game](https://colab.research.google.com/github/bikegirl/IFaTG/blob/master/HW2/my_game_improved.ipynb)
