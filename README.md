## MORSE_CODE-CONVERTOR
# OVERVIEW OF PROJECT
That​‍​‌‍​‍‌​‍​‌‍​‍‌ is an excellent point. Why don't we explore a bit more why Morse code has to deal with that particular spacing problem which most of the time is a big barrier for those who learn the code.

Why is the Spacing So Important?

Think over it: if you were to talk with somebody, but talking in that way which is a steady, continuous stream and without any sort of pausing for words or even syllables, no doubt that one person wouldn't understand you at all.

Morse code is just like that, however, unlike the sound of our voice by which if we want to take a pause (for a breath) we indicate it, here it is silence or empty space which is used between the dots and dashes to show the pause. So the receiver must be very sure that the first character is terminating and the next one is starting.

The standard system relies on the time it takes to send one short dot (\text{.}):

 Element - Description - Duration (in Dot-Units) .



Dot (\text{.}) :The basic unit of sound (or light). (1 Unit )

Dash (\text{-}): A long sound (three times longer than a dot). ( 3 Units )

Inner Character Space :The silence between the dots and dashes of a single letter (e.g., between the dot and dash in \text{A} which is \text{.-}). | 1 Unit |

 Letter Space  The silence between two different letters (e.g., between \text{H} and \text{E}).( 3 Units)

 Word Space  The silence between two different words. ( 7 Units )

First of all, I think it's important that you understand how a morse code generator works, because it could give you an idea of why it is treating spacings in such a very specific moronic way.

When a Morse code generator like the Python program is producing the output string, it's not physically putting 7 blanks in a row to indicate a word space; rather, the representation of the huge gap is being put there.

* We used three spaces ( ) as the word break in our Python example.

* The one who gets this output (or the translator software) is aware that three spaces stand for, "Wait, an entirely new word is coming here!"

In case the generator had gone wrong in the use of the extended word space, and instead of a single space (1 unit of time) that separated the words a person had put them together, the receiver would merge the last letter of the first word with the first letter of the second word without realizing it and therefore transforming the saying "HELLO WORLD" into a string of that is totally incomprehensible.

It means, therefore, that the crux of the generator's work is not only the dictionary lookup but also, and probably more importantly, the accurate performance of the proper pauses (spaces) so as to be able to retain the encoded message's readability and evenness.
# FEATURES
* THE OUTMODES ( RECEIVE THE CODE )
  1. AUDIO  (BEEPS)
  2. VISUAL (FLASHES)
  3. TEXT  (DOTS AND DASHES)
* SPEED AND TIME CONTROLS
* HANDLING INPUT AND CHARACTERS
  1. PUNCTUATION AND NUMBERS    
  2.UNSUPPORTED CHARACTERS
  3. REAL TIME GENERATIONS
* PRACTISE AND ADVANCED
# TECNOLOGY AND TOOLS
You're​‍​‌‍​‍‌​‍​‌‍​‍‌ trying to make this sound like a conversation a little more casual between two people! No problem, let's forget the manual and just talk about how this translator works.

 The Morse Code Translator: Talking Like a Friend

Forget "tools" and "modules." Here's how the Python program does the work—it's as if you had three friends supporting you.</li></ul>1. The Dictionary: Your Cheat Sheet 

This is the brain of the whole operation, but really, it's just a cheat sheet (or a massive list) inside the computer's memory.

Job: To know everything. It has the official, secret handshake (the code) for every single character.How it works: Say you are translating the word "SNAKE."The code asks the Cheat Sheet: "Hey, what's 'S'?"The Cheat Sheet immediately answers: It's the ultimate flashcard deck, except the computer never has to shuffle or forget.iDecoding: If you give it the code .-, it instantly knows, "Oh, that's 'A'." It can translate both ways immediately.2. Strings & Splitting: The Message Editor 

It's the one who understands your writing, and knows just the right place to cut it up, especially because Morse code has very specific gaps.

: Taking the big, long text and breaking it into bite-sized pieces so the Cheat Sheet can read it.Going English to Morse: The Editor just scans your message, letter by letter. "Okay, I'm done with 'H'... now move to 'E'." (This is the simple for loop).Going Morse back to English: This is where the Editor gets the most work, because it deals with the strange spaces:If he sees a small gap (one space): "Alright, that's just the end of a letter. Let me put that letter aside."If he sees a huge gap (three spaces): "Whoa! That was a whole word! Time for a proper pause before I start the next word's translation." In this way, the words of yours do not get mixed up unintentionally.3. Time and Sleep: The Pacer 

In case you want the computer to beep the Morse code out loud, the Pacer is definitely the one creating the rhythm that you need.

Job: Making sure the sounds are timed perfectly, just like a conductor guiding an orchestra.How it works: It implements a very simple command that essentially means: "Hey, computer! Do nothing for exactly 0.1 seconds."For a Dot: "Make a quick beep, then do nothing for a moment."For a Dash: "Make a longer beep, then do nothing for three times longer."This little "do nothing" pause is the entire secret to Morse code timing. It ensures that when you hear the code, you know exactly what is a dot, what is a dash, and where the words start and ​‍​‌‍​‍‌​‍​‌‍​‍‌end.
# 
