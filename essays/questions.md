---
layout: essay
type: essay
title: How to Get Answers to Your Questions
# All dates must be YYYY-MM-DD format!
date: 2019-01-24
labels:
  - Effective questions
---
How to Get Answers to Your Question
====

>"There are naive questions, tedious questions, ill-phrased questions, questions put after inadequate self-criticism. But every question is a cry to understand the world. There is no such thing as a dumb question."
Carl Sagan

Dr. Sagan had a great view on questions: They are just a way of trying to better understand the world. No matter how trivial or outlandish they may be, a question is a request for better understanding, and should not be scoffed at. Unfortunately, this logic is not shared by the some of the people you will sooner or later come into contact with when trying get assistance with a bug, or whatever other problem you may find in your computer science career. Hell hath no fury like a person behind  a keyboard, so to prevent you from feeling this wrath, I present a few examples of _*effective*_ questions, and _*ineffective*_ questions


Ineffective
----
>i want to return a double however it always returns an integer. this code returns 10.0, I want the decimals as well

>I have tried using a different public variable,



```Javascript
     public double getCost()
        {
            double price = 500/46; 
            return price;
        }
  ```
  
  
 >I want to get decimals. I hope to get 10.869...
 
 
 This question seems pretty solid, the verbiage is easy to understand, code is formatted so that it is easy to read, and he even posts what his desired return value is. This question becomes a bad question in that a quick search of "The Java Tutorials" on Oracle's website could have provided the necessary information much faster than posting and waiting for a response.
 
 ----
 
 >Hello Frineds,

>I having been recived a task to craete this iphone APPLICATION which can connect to a website and send information to database. Also >must store an imgae on data base and on phone. Pleas tell me how to do this. Must know very soon.

>thanks you all

This question I found in Meta StackExchange under a thread called "What is a "Bad" question". Answering this question would require a textbook. There is no way of determining what level of knowledge the individual who asked the question has. Is he a novice programmer, trying to understand at a high-level view? Perhaps an expert who encountered a bug? Intuition leads us to the first answer, but we have no way of knowing for sure. The second thing I notice is spelling. It's always a good idea to run a spell-check with any one of the many online text-editors available. I found this free one: (https://www.online-spellcheck.com/) in about 3 seconds. The final thing to note from this post is the phrase "Must know very soon." Ending a question with how urgently you need an answer will not cause the question to be answered any faster, thus it's trivial to set an urgency level on your question.

Effective
-----

>How to access range of bits in a bitset?

>I have a bitset which is very large, say, 10 billion bits.

>What I'd like to do is write this to a file. However using .to_string() actually freezes my computer.

>What I'd like to do is iterate over the bits and take 64 bits at a time, turn it into a uint64 and then write it to a file.

>However I'm not aware how to access different ranges of the bitset. How would I do that? I am new to c++ and wasn't sure how to access >the underlying bitset::reference so please provide an example for an answer.

>I tried using a pointer but did not get what I expected. Here's an example of what I'm trying so far.

```
#include <iostream>
#include <bitset>
#include <cstring>
using namespace std;

int main()
{
    bitset<50> bit_array(302332342342342323);
    cout<<bit_array << "\n";
    bitset<50>* p;
    p = &bit_array;
    p++;
    int some_int;
    memcpy(&some_int, p , 2);
    cout << &bit_array << "\n";
    cout << &p << "\n";
    cout << some_int << "\n";

    return 0;
}

```

>the output:

````
10000110011010100111011101011011010101011010110011
0x7ffe8aa2b090                                                                                                                          
0x7ffe8aa2b098
17736
````
>The last number seems to change on each run which is not what I expect.

This is an example of a great question. His question is clear and concise, with neatly formatted code. He gives a description of methods he has attempted, so the people that may potentially help him don't waste their time attempting them, or better yet, can provide him feedback on how those implementations may work. He even gives an example of the results he is receiving, so people can compare their implementations with his. Overall, A+ question.

The saying "There are no stupid questions" still holds true, but there are effective and ineffective questions. Hopefully after viewing these examples, you can ask questions that will get you better answers, and sooner. So, don't be afraid to post the questions you may have, just take the time to make sure you're conveying them in an_* effective*_ manner.
