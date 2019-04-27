As I've progressed in my software developer career, I've learned, often the hard way, that **doing things in certain ways was more productive, increased quality, and facilitated cooperation with my teammates**.

At some point I've started thinking about programming as a *craft*. Extremely hard to master, evolving quickly, and very demanding. Let me show you the definition of a *craftsman* from the online Cambridge English Dictionary:

> Craftsman – a person who is skilled, especially someone who makes things by hand

<p class="quoteSource"><a href="https://dictionary.cambridge.org/us/dictionary/english/craftsman#dataset-cbed">source: Cambridge Dictionary</a></p>

I really like the sound of that. Aren't software developers the craftsmen of the 21<sup>st</sup> century?

This document is a conclusion of my findings related to working as a software developer. I believe that the ideas presented in this document will allow a developer to progress towards becoming a master craftsman in the land of software development. All topics presented here are technology-agnostic, meaning that it doesn't matter which programming language or framework is your domain.

I've divided the document into *Elements*, grouped by topics they relate to. I really liked the idea of *"Items"* in Joshua Bloch's astounding *Effective Java* book. The author clearly presented a way-to-go for various Java programming paradigms and problems in his *Items*. I came up with the notion of *Elements*, which are, in my opinion, a foundation for becoming a master craftsman. I myself am nowhere near to becoming one, yet, but I feel I'm on the right course.

All ideas presented here are just my thoughts. I'm basing them on experience gained on many projects I have been working on over the years – maybe you will agree with me on some of them, and disagree on other. I'd like to know what you think about them, and it would be great if you would share your thoughts – I'll happily receive any e-mails: <przemyslaw.kruglej@gmail.com>.

# <a name="listOfElements"></a>Elements of Craftsmanship of Software Development

* [Elements of Quality](#elementsOfQuality)
  * [Element 1 – Have Your Code Reviewed](#element1HaveYourCodeReviewed)
  * Element 2 – Make Quality Your Driving Force
  * Element 3 – Care About Small Things
  * Element 4 – Be Reliable

## <a name="elementsOfQuality"></a>Elements of Quality

This group of elements relates to the quality of software developer's work.

### <a name="element1HaveYourCodeReviewed"></a>Element 1 – Have Your Code Reviewed

How many times have you seen code that wasn't complying with your project's style guide ([Element 16 – Comply with Project's Code Style Guide](#element16ComplyWithProjectsStyleGuide)), didn't conform with the best practices, had bugs in plain sight, and just wasn't well written? All of those could have been spotted and fixed during a code review. So, why weren't they? The problem here is threefold.

Firstly, people fear criticism, and that's what often code review ends up being. On the other hand, well-done code review (Element 14 – Put Effort in Code Reviews) facilitates better code quality and lowers number of bugs, and in my opinion quality should be our driving force (Element 2 – Make Quality Your Driving Force).

<span class="textImportant">If this is the case for you, don't be afraid of code reviews. Find people on your project that you know will provide constructive feedback and that will make effort to help you improve your code.</span>

Secondly, some developers tend to overlook one simple truth: everyone makes mistakes (which every introduced bug confirms). Be humble – no matter how much experience you have, your code is not error-proof. We all make mistakes, and there is no shame in having somebody point out a problematic piece of our code **during a code review**.

<span class="textImportant">Give others a chance to spot a bug in your code before it goes to production.</span>

Lastly, some developers are just not used to code reviews, and often don't realize how much good it can bring them to have someone take a look at their code. Keep in mind that each code reviewer always has a different perspective, which includes different skills, experience, and project knowledge. They will see things that might be improved and/or that are vital to the project you are working on.

<span class="textImportant">Make it a habit of having your code reviewed. It does pay off, and increases quality of the code you create.</span>

To summarize, code review is a great tool that can help you increase quality of your code and minimize number of bugs in your code. <span class="textImportant">You just need to give your teammates a chance to do it.</span>

<p class="backToToC"><a href="#listOfElements">&gt; back to the Elements' list</a></p>