# MORSE_CODE-CONVERTOR
# OVERVIEW
That​‍​‌‍​‍‌​‍​‌‍​‍‌ is an excellent point. Why don't we explore a bit more why Morse code has to deal with that particular spacing problem which most of the time is a big barrier for those who learn the code.

Why is the Spacing So Important?

Think over it: if you were to talk with somebody, but talking in that way which is a steady, continuous stream and without any sort of pausing for words or even syllables, no doubt that one person wouldn't understand you at all.

Morse code is just like that, however, unlike the sound of our voice by which if we want to take a pause (for a breath) we indicate it, here it is silence or empty space which is used between the dots and dashes to show the pause. So the receiver must be very sure that the first character is terminating and the next one is starting.

The standard system relies on the time it takes to send one short dot (\text{.}):

| Element | Description | Duration (in Dot-Units) |



| Dot (\text{.}) | The basic unit of sound (or light). | 1 Unit |

| Dash (\text{-}) | A long sound (three times longer than a dot). | 3 Units |

| Inner Character Space | The silence between the dots and dashes of a single letter (e.g., between the dot and dash in \text{A} which is \text{.-}). | 1 Unit |

| Letter Space | The silence between two different letters (e.g., between \text{H} and \text{E}). | 3 Units |

| Word Space | The silence between two different words. | 7 Units |

First of all, I think it's important that you understand how a morse code generator works, because it could give you an idea of why it is treating spacings in such a very specific moronic way.

When a Morse code generator like the Python program is producing the output string, it's not physically putting 7 blanks in a row to indicate a word space; rather, the representation of the huge gap is being put there.

* We used three spaces ( ) as the word break in our Python example.

* The one who gets this output (or the translator software) is aware that three spaces stand for, "Wait, an entirely new word is coming here!"

In case the generator had gone wrong in the use of the extended word space, and instead of a single space (1 unit of time) that separated the words a person had put them together, the receiver would merge the last letter of the first word with the first letter of the second word without realizing it and therefore transforming the saying "HELLO WORLD" into a string of that is totally incomprehensible.

It means, therefore, that the crux of the generator's work is not only the dictionary lookup but also, and probably more importantly, the accurate performance of the proper pauses (spaces) so as to be able to retain the encoded message's readability and evenness.

Would you want to have a go at a brief sentence and translate it into Morse code by applying the rules we have just talked ​‍​‌‍​‍‌​‍​‌‍​‍‌about?
