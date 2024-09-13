---
layout: essay
type: essay
title: "Do Dumb Questions Exist?"
# All dates must be YYYY-MM-DD format!
date: 2024-09-11
published: true
labels:
  - Questions
  - Answers
  - StackOverflow
---

<img width="300px" class="rounded float-start pe-4" src="../img/smart-questions/rtfm.png">

## Why Ask Questions?

Asking questions is fundamental especially for learning and for personal growth. It is a crucial part of communication which is a very important aspect in becoming a software engineer. As we begin to learn new things it is natural to be curious and asking questions is a way to satisfy that curiosity. We have been asked the question, "Do dumb questions exist?" and the answer to that is no. Every question, when asked with genuine curiosity and the intent to learn, has value. The most important aspect is creating a meaningful and effective question that leads to a satisfying and informative answer. 

## What is a NOT SO SMART question?

As a software engineer or programmer, there are many forums such as StackOverflow where you can ask a question and receive feedback from others. There have been times when we have asked questions and did not receive the exact answer we were looking for. This is likely because the question that was asked was not so smart. Before asking questions on online forums, we should make sure that our questions are not easily answered through simple google searches. We should also make sure that our question is specific and asked in a way for us to receive a proper response. By doing this, we can save not only other people's time, but also our own time trying to get responses from others. Here is an example of a <a href="https://stackoverflow.com/questions/35683216/whats-the-output-of-this-code-written-in-java">not so smart question.</a> 

```
Q: What's the output of this code written in java?

        int arr[ ] = new int[3];
    for (int i = 0; i < 3; i++) {
       arr[i] = i;
    } 
    int res = arr[0] + arr[2];
    System.out.println(res);

```


A user posted this question on stack overflow for the output of a simple java code. The user could easily have gotten the output by compiling and executing their own code. Later on, the user mentioned that they actually wanted to understand what was going on with the code and how it actually came up with that output, but the question itself did not really specify that. If the user also put some effort into google searching, the user can also understand how the code functions and produce a certain output.

## What is a SMART question?

On the other hand, SMART questions is easy to follow and understand, shows effort and highlights the problem at hand. SMART questions also demonstrate that there was effort put in as well wether it be what they searched on google, or what they did to try and and solve the question on their own. Here is an example of a <a href="https://stackoverflow.com/questions/11227809/why-is-processing-a-sorted-array-faster-than-processing-an-unsorted-array">smart question.</a> 

```
Q: Why is processing a sorted array faster than processing an unsorted array?

In this C++ code, sorting the data (*before* the timed region) makes the primary loop ~6x faster:

#include <algorithm>
#include <ctime>
#include <iostream>

int main()
{
	// Generate data
	const unsigned arraySize = 32768;
	int data[arraySize];

	for (unsigned c = 0; c < arraySize; ++c)
		data[c] = std::rand() % 256;

	// !!! With this, the next loop runs faster.
	std::sort(data, data + arraySize);

	// Test
	clock_t start = clock();
	long long sum = 0;
	for (unsigned i = 0; i < 100000; ++i)
	{
		for (unsigned c = 0; c < arraySize; ++c)
		{	// Primary loop.
			if (data[c] >= 128)
				sum += data[c];
		}
	}

	double elapsedTime = static_cast<double>(clock()-start) / CLOCKS_PER_SEC;

	std::cout << elapsedTime << '\n';
    std::cout << "sum = " << sum << '\n';
}

- Without `std::sort(data, data + arraySize);`, the code runs in 11.54 seconds.
- With the sorted data, the code runs in 1.93 seconds.


(Sorting itself takes more time than this one pass over the array, so it's not actually worth doing if we needed to calculate this for an unknown array.)


Initially, I thought this might be just a language or compiler anomaly, so I tried Java:

import java.util.Arrays;
import java.util.Random;

public class Main
{
	public static void main(String[] args)
	{
		// Generate data
		int arraySize = 32768;
		int data[] = new int[arraySize];

		Random rnd = new Random(0);
		for (int c = 0; c < arraySize; ++c)
		    data[c] = rnd.nextInt() % 256;

		// !!! With this, the next loop runs faster
		Arrays.sort(data);

		// Test
		long start = System.nanoTime();
		long sum = 0;
		for (int i = 0; i < 100000; ++i)
		{
			for (int c = 0; c < arraySize; ++c)
			{  	// Primary loop.
				if (data[c] >= 128)
					sum += data[c];
			}
		}

		System.out.println((System.nanoTime() - start) / 1000000000.0);
		System.out.println("sum = " + sum);
	}
}

With a similar but less extreme result.

---

My first thought was that sorting brings the data into the [cache](https://en.wikipedia.org/wiki/CPU_cache), but that's silly because the array was just generated.

- What is going on?
- Why is processing a sorted array faster than processing an unsorted array?

The code is summing up some independent terms, so the order should not matter.
```


In this SMART question, the user is asking "Why is processing a sorted array faster than processing an unsorted array?" The user clearly demonstrates that they put effort into the question through test cases and their results, comments on code that explain what is going on, making it easier to follow as well as what the user predicts to be occuring in the code to make processing sorted arrays faster than unsorted arrays. By creating a smart question, the user was able to receive hundreds of clear and detailed answers/solutions to the question. 

## Ask Smart Questions

Overall, in software engineering, it is vital to ask smart questions as we are more likely to receive the answer that we are looking for. Through my experience on StackOverflow, I found out that you are able to receive a much more detailed and satisfactory response if you take your time and show effort in the questions that you are asking. Asking smart questions can greatly enhance your learning experience and boost your communication skills. 
