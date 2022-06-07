# Lab 15: Labrador Giveaways

[GitHub Classroom assignment](https://google.com)

## 0. Intro

The purpose of this lab is twofold: to serve as a handy _base_ template for other lab handouts, and to teach you some tricks of the trade! You will get to try your hand at doing certain things like XYZ and ABC, and (hopefully) learn something new in the process. It might also help with your projects (i.e. handouts and algos) :wink:.

In the rest of this 1-2h lab (NB: actually 5 min), you will:

1. Think about how to effectively communicate learning objectives, task instructions, and more,
2. Experiment with using GitHub Markdown to format things (including math equations!), and
3. Lorem ipsum some dolor sit amet.

> Don’t like numbered lists in an introduction? If all of you hate it, feel free to use regular prose instead.

## 1. Effective Written Communication

At this point, you might already have a sense of the content your lab will contain. That said, knowing _what_ to teach is only half the battle---there still remains the question of _how_ to teach it.

Here are some tricks that you can and should use in your own handout-writing:

### 1.1. Declaring Intent

Notice that, in section 0, we made it very clear what the point of this lab was. And we might even repeat it again in a later section like this one: this lab is a starting point and guide for your own handouts.

Declaring intent explicitly is something most good instructional materials do, as it [primes](https://en.wikipedia.org/wiki/Priming_(psychology)) learners to keep certain end-goals in mind. For a comparison, consider how you might watch a movie when you already know a critical plot twist: often, this leads you to pay more attention to clues and details that lead into that story beat.

**Task**

For reference, take a quick look at the first few paragraphs of this [CSCI 0300 lab handout](http://cs.brown.edu/courses/csci0300/2021/assign/labs/lab3.html) (among other equally good ones).

What do they do to make the concept of the lab clear? (Write down a response for your lab checkoff, later)

### 1.2. Using Hierarchies and Heading Levels

A more subtle way to improve written communication is to use hierarchies and heading levels to help students group up concepts mentally.

Combined with the explicit intent, headers can be used to succinctly capture the purpose and content of entire sections of a handout; this reduces the number of things that need to be held in students’ working memory while they’re parsing different parts of the handout, and thus increases their rate of information uptake.

The catch is that these hierarchies must make logical sense and use consistent language, or else the discordance would cause confusion (and ultimately it’d be a net negative).

> An aside: at a very high level, this is rather similar to trees (the data structure). Trees are great because they preserve locality and permit easy lookup and pruning. As an added bonus, CS students are used to reading text formatted like trees---after all, that’s what most indented code looks like!

**Task**

Reorganize the following list of steps into a more hierarchical structure. Feel free to change the precise wording of each section/subsection.

Uh oh! The image below is broken...

```
![This is alt-text for an image which doesn’t exist](path/to/non-existent/image)
```


![This is alt-text for an image which doesn’t exist](path/to/non-existent/image)


## 2. GitHub Markdown Formatting

Speaking of broken formatting, let’s explore the features and functionality of GitHub Markdown!

### 2.1. Markdown Math

GitHub Markdown math support is relatively new, and in our opinion, very much untested. But y’all voted for it... and we gotta work with what we got.

What’s cool is that it supports inline math like $ y = mx + b $ and symbols like $ \gamma $, but also block-level math, like this:
 
$$
  I_λ = K_a O_{aλ} \\
    + \sum_{m=0}^{\text{numLights}-1} \left[ I_{mλ} \cdot (k_d O_{dλ} \hat{n}) \cdot \hat{L_m} \right]
$$

**Task**

Try it yourself! Typeset the following expressions:

```
1. sum of (i^2) for i from 0 to 10 inclusive
2. todo
```

> Hint 1: remember to use `$$` delimiters. We recommend using them on the line before and after your equation, for readability.
>
> Hint 2: you can align multi-line equations using `\begin{align}` and `\end{align}`.

### 2.2 Collapsible Sections

Of course, typesetting math can be done (much simpler) in LaTeX proper. Where GitHub Markdown truly shines is in its web setting, which allows for (some) interactivity.

In this section, you will learn how to hide extra information for students to read!

<details>
  <summary>How exactly can I do that?</summary>

  Like this!
 
  ```
  <details>
    <summary>How exactly can I do that?</summary>
  
  Like this!
  
  </details>
  ```
  
</details>

<details>
  <summary>Why would I want to do that?</summary>

  Sometimes lab handouts can get really long, so collapsible sections can save space by hiding optional info and recaps.

  As we have very little stylistic (i.e. CSS) control over GitHub Markdown, this is one of the very few (and most powerful) tools at our disposal for improving readability. Feel free to use it often, but do so intelligently!
  
</details>

**Task**

Write a collapsible section containing your own secret knowledge below.

> Hint: remember to use the `<details>` and `<summary>` tags!

## End

> Didn’t you learn so much from this lab?
> 
> So cool!

Go get checked off by a TA!

Here are some questions to answer:

- How awesome is CSCI 1230?
- What percentage of that is due to what you’re going to be doing this summer? (There is a correct answer, and it is a positive, non-zero integer multiple of 100)
- Which lab is your favorite? 




