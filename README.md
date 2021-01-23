# vegan-hacktivists-challenge
Vegan Hacktivists coding challenge






# About Challenge

Hey!

First off, thank you for taking the time to do this challenge. We know it's annoying, but there are a few reasons we now require this before being accepted into the Vegan Hacktivists. First, a number of volunteers in the past, while passionate, didn't have much programming experience. This led to a decrease both in code quality and available time from the more senior developers (due to answering questions, refactoring, etc.). The bigger issue, however, is that many of our volunteers have disappeared without warning, leaving us shortstaffed. With this coding challenge, we're hoping to narrow our recruitment down to those with both experience and the will to put in some work.

The challenge shouldn't take more than an hour or two, assuming you have an environment set up for PHP development. That being said, take as much time as you need to complete it. You can even add extra bells and whistles if you want, but it is absolutely not required; **we're going to be looking at the quality of your code, so make that your main focus.**

After submitting the challenge, we will review it to determine whether or not we think you'd be a good fit to join us.

## The challenge

The goal is to build a very, very simple Q&A website. A visitor should be able to ask questions and leave answers without any authentication. How you set up the routes and whatnot is up to you, but at the very least, the website should contain:

1. A page showing list of questions
2. A page to view one question, including its answers
3. Forms for submitting a question and an answer

[Here is an example](https://challenge.veganhacktivists.org). **It does not need to look exactly like this.**

## Hard requirements

1. The website **must** be built using Laravel and MySQL.
2. The forms **must** be validated. If a form fails validation, it must stay populated, rather than getting reset.
  * Question validation:
    * Required
    * Minimum length: 5
    * Ends with a question mark ("?")
  * Answer validation:
    * Required
    * Minimum length: 5
3. The textarea/input for questions **must** display a random question for the placeholder. The random questions are up to you to write! Feel free to have fun with it.
4. The list of questions **must** be sorted from **newest to oldest**.
5. A question's list of answers **must** be sorted from **oldest to newest**.

## Soft requirements

* To the best of your abilities, use Bootstrap as much as possible and avoid writing custom styles. The demo submission linked to above contains no custom CSS.
* Try to make it look decent. You don't need to be a pro designer, but we've found it difficult to find UI designers, so the ability to make things presentable is a huge plus.

## Tips

* Laravel and Bootstrap have a ton of functionality built-in. If you find yourself writing some custom code for something like getting a random element from an array or adding margins to an element, you may want to take a closer look at the documentation :grin:
* Not a requirement, but nested resources are great. `POST /questions/:question_id/answers` is better than `POST /answers`, and it's easier to code it that way!

## What we'll be looking at

* Good Git commit history
* Clean, understandable code
* Either clear experience with the technology we use (namely Laravel and Bootstrap) or the ability to pick them up quickly by referring to the documentation

## Submission

Please send us a link to a GitHub repository that we can view. If you'd like to host a demo somewhere (e.g. Glitch, Heroku, etc.), feel free to send that too, but it is not required at all.