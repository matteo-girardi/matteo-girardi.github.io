---
layout: post
title:  "It takes too much time, I won't write unit tests."
date:   2020-09-15 18:23:36 +0200
categories: TDD
---

Halløj! 👋

In today's post, I'd like to talk about the importance of Test Driven Development (TDD) in software development. I won't give any code snippets and I won't talk in details about TDD, SOLID, KISS and other important principles and practises. It's essential to know what they are, however in this post I'd just like to focus on why TDD is important and underline the relevance of writing tests.

I'd like to do so because the other day I heard the following sentence: 

- **"It takes too much time, I won't write unit tests."**

It doesn't matter who said it and where it was said. In fact, it may even be *fugazi*.

I know that we, as software developers, have been talking, reading, and learning about this topic over and over again, but it looks like we don't trust the practice of writing tests. Or perhaps we do trust it, though we are pushed to deliver fast instead of deliver quality, and therefore we take shortcuts.

My advice is as follows:

- **write tests, no matter what it takes!**

I know it sounds harsh... but the truth, I believe, is pretty clear. If you don't write tests, you are not and will never be confident with the code you write.

- **no TDD, no confidence, no proof that your code is working as expected**

that's it! This is the reason why TDD is *fundamental*.

You can of course say:
> I've tested all the scenarios myself and it works.

Fair enough. <br />
Well, let's say that one of the API you rely on is going to change. Are you going to re-test all the scenario and possible new scenarios yourself? or would you rather like to have a well automated suite of tests ? 

I know what I would choose 🙂

Consider the following example: <br />

> You started a brand new project few years ago, and it got bigger and bigger. You haven't written that many tests, and it isn't necessarily a bad thing. It could be that the tests you wrote cover enough code, they test only what need to be tested and you feel confident.

*too good to be true*. 

> The tests you wrote are not even close to be enough, you wrote tests here and there, when you felt like it. And let's imagine you have been using *"some-kind-of-anti-pattern"* extensively, which makes your code tightly coupled together, difficult to test (that's why you haven't written that many tests) and it looks like everything is responsible for everything. Whenever you wrote some tests, you did so *AFTER* you implemented a new feature. By doing so, you haven't taken into consideration all the dependencies you have and probably you wrote code that isn't testable. 

Well, I believe that this is the **recipe for disaster**. <br />

I believe that following TDD and writing unit tests is never, ever, a waste of time. It is an investment in the future, actually.
No matter how much time and effort it takes, writing tests and following TDD will make you confident with the code you write.

- *Make a commitment* and follow TDD.

I won't provide links to any resources, because you just need to google TDD, unit tests, Extreme Programming, Dependency Injection, SOLID, etc.. You will find plenty of books, articles, tutorials and more. 

I'll end with a motto:

- **In TDD we trust**

till next time.. 

Hygge!
