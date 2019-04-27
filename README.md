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
  * [Element 2 – Make Quality Your Driving Force](#element2MakeQualityYourDrivingForce)
  * [Element 3 – Care About Small Things](#element3CareAboutSmallThings)
  * [Element 4 – Be Reliable](#element4BeReliable)
* [Elements of Versatility](#elementsOfVersatility)
  * [Element 5 – Search for Answers](#element5SearchForAnswers)
  * [Element 6 – Acknowledge Testing as a Part of Your Job](#element6AcknowledgeTestingAsPartOfYourJob)
  * [Element 7 – Look at the Bigger Picture](#element7LookAtTheBiggerPicture)
  * [Element 8 – Embrace the Challenge of Other Technologies](#element8EmbraceTheChallengeOfOtherTechnologies)
* [Elements of Teamwork](#elementsOfTeamwork)
  * [Element 9 – Think About Developers Who Will Maintain Your Code](#element9ThinkAboutDevelopersWhoWillMaintainYourCode)
  * [Element 10 – Value Time of Other People by Asking the Question the Right Way](#element10ValueTimeOfOtherPeopleByAskingTheQuestionTheRightWay)
  * [Element 11 – Be Helpful](#element11BeHelpful)
  * [Element 12 – Don't Blame – Solve Problems](#element12DontBlameSolveProblems)
  * [Element 13 – If Things Go Wrong, Admit It](#element13IfThingsGoWrongAdmitIt)
  * [Element 14 – Put Effort in Code Reviews](#element14PutEffortInCodeReviews)
  * [Element 15 – Document Your Work and Provide Helping Information for Testers](#element15DocumentYourWorkAndProvideHelpingInformationForTesters)
  * [Element 16 – Comply with Project's Code Style Guide](#element16ComplyWithProjectsCod StyleGuide)
  * [Element 17 – Read What You Wrote Before Hitting "Send"](#element17ReadWhatYouWroteBeforeHittingSend)
* [Elements of Version Control](#elementsOfVersionControl)
  * [Element 18 – Care for the Code Repository](#element18CareForTheCodeRepository)
  * [Element 19 – Master Your Version Control System](#element19MasterYourVersionControlSystem)
  * [Element 20 – Write Descriptive Commit Messages](#element20WriteDescriptiveCommitMessages)
  * [Element 21 – Break Changes Into Commits](#element21BreakChangesIntoCommits)

## <a name="elementsOfQuality"></a>Elements of Quality

This group of elements relates to the quality of software developer's work.

### <a name="element1HaveYourCodeReviewed"></a>Element 1 – Have Your Code Reviewed

How many times have you seen code that wasn't complying with your project's style guide ([Element 16 – Comply with Project's Code Style Guide](#element16ComplyWithProjectsStyleGuide)), didn't conform with the best practices, had bugs in plain sight, and just wasn't well written? All of those could have been spotted and fixed during a code review. So, why weren't they? The problem here is threefold.

Firstly, people fear criticism, and that's what often code review ends up being. On the other hand, well-done code review ([Element 14 – Put Effort in Code Reviews](#element14PutEffortInCodeReviews)) facilitates better code quality and lowers number of bugs, and in my opinion quality should be our driving force ([Element 2 – Make Quality Your Driving Force](#element2MakeQualityYourDrivingForce)).

<span class="textImportant">If this is the case for you, don't be afraid of code reviews. Find people on your project that you know will provide constructive feedback and that will make effort to help you improve your code.</span>

Secondly, some developers tend to overlook one simple truth: everyone makes mistakes (which every introduced bug confirms). Be humble – no matter how much experience you have, your code is not error-proof. We all make mistakes, and there is no shame in having somebody point out a problematic piece of our code **during a code review**.

<span class="textImportant">Give others a chance to spot a bug in your code before it goes to production.</span>

Lastly, some developers are just not used to code reviews, and often don't realize how much good it can bring them to have someone take a look at their code. Keep in mind that each code reviewer always has a different perspective, which includes different skills, experience, and project knowledge. They will see things that might be improved and/or that are vital to the project you are working on.

<span class="textImportant">Make it a habit of having your code reviewed. It does pay off, and increases quality of the code you create.</span>

To summarize, code review is a great tool that can help you increase quality of your code and minimize number of bugs in your code. <span class="textImportant">You just need to give your teammates a chance to do it.</span>

<p class="backToToC"><a href="#listOfElements">&gt; back to the Elements' list</a></p>

### <a name="element2MakeQualityYourDrivingForce"></a>Element 2 – Make Quality Your Driving Force

When you start working on a task, what do you picture as the end result? Is it just a trio of: a commit, deployment, and time spent logged in an issue tracker?

Let me propose a different approach, where you care about the value of the delivered piece of software from the very beginning, and all you do, you do with one thing in mind.

Quality.

This might sound simply, but it takes time to get into the habit of this approach, which I call *Quality-Driven Development*.

Whenever you start working on a task, keep in mind that your approach is quality-driven. <span class="textImportant">Your goal is to end up with a piece of software that you will be proud of.</span> **Remember that your name will be next to the commits which introduce changes in the project.** And that alone, in my opinion, is a very powerful notion, worth stopping for a moment and thinking about. Consider that from the moment when you push your changes, everyone will be able to see them, and <span class="textImportant">though you can't judge a book by its cover, the same cannot be said about source code and its author</span>.

Therefore, **make quality your driving force**. <span class="textImportant">Whenever you deliver something, ask yourself these simple questions:</span>

<ul class="listWithMargin">
  <li><em>"Is this the best I could have done?"</em> – Can you say that this piece of code couldn't have been done better, taking your skills and knowledge into consideration?</li>
  <li><em>"Have I left nothing behind?"</em> – Are all of the cases, that you have thought of, taken into account?</li>
  <li><em>"Could I have asked somebody to help me improve my code?"</em> – If you know there is somebody on your project that could help you improve your code, have you asked for their expertise?</li>
</ul>

Many of the other Elements in this document emphasise directly, or indirectly, *Quality-Driven Development*, and propose ways to support it, like [Element 3 – Care About Small Things](#element3CareAboutSmallThings) or [Element 9 – Think About Developers Who Will Maintain Your Code](#element9ThinkAboutDevelopersWhoWillMaintainYourCode).

<p class="backToToC"><a href="#listOfElements">&gt; back to the Elements' list</a></p>

### <a name="element3CareAboutSmallThings"></a>Element 3 – Care About Small Things

Sometime you encounter a task (perhaps even yours) and you notice that it could have been done better.

<ul class="listWithMargin">
  <li>Maybe the author hasn't paid enough attention to the code formatting, or the code violates some of the best-practices used on the project, or the code has been written in a way that is hard to understand.</li>
  <li>It might be that the tests haven't been written or updated, or no attention was paid to what happened to the task after it has been merged (and something went wrong), or the commit message isn't descriptive.</li>
  <li>Perhaps some of the business cases were neglected by the developer, because he either thought they were close-to-nonexistent, or because they were not included in the business specification, and the developer didn't think about mentioning them to the business users.</li>
  <li>Maybe the related documentation hasn't been updated after the task had been done, or information that would help testers perform the test of the task hasn't been supplied.</li>
</ul>

The points listed above (and other, as the list could go on and on) would be regarded differently by each developer. Some would be negligible, whereas other would be requirements in the *definition of done*. Either way, they can all be viewed as details. And <span class="textImportant">details make all the difference.</span> **It is the small things that bring a developer's work to the next level.**

<span class="textImportant">Don't leave anything behind. Whenever you feel like the task is ready, consider if there is anything that you can improve, or if there is any related action that you can do.</span>

There is another important thing to mention here, and a separate *Element* is dedicated to it. <span class="textImportant">People notice detailed work and quality code, and, therefore, its author</span>, and it is a good feeling being regarded highly by your colleagues ([Element 4 – Be Reliable](#element4BeReliable)).

So <span class="textImportant">pay attention to the details. They all add up to the quality of what you deliver.</span>

One thing, however, that working on the details requires, is time. It is often a trade off between how much time you have and how strongly you feel about delivering top quality. Keep in mind that making your tasks *pixel-perfect* will often take significantly more time. It might not always be the right solution and you will have to adapt (adaptation is [the topic of the next set of Elements](#elementsOfVersatility)). Try finding a middle ground when needed.

<p class="backToToC"><a href="#listOfElements">&gt; back to the Elements' list</a></p>

### <a name="element4BeReliable"></a>Element 4 – Be Reliable

When you join a new project, you often find out that there are some people that are said to *know everything* related to the project and/or are very strong from the technical point of view, and you can always ask them for an advice, learn from them, and expect their work to be of finest quality.

You can be such a person. All it takes is the *Quality-Driven Development* approach, attention to details, technical expertise, and being helpful... Sounds like a lot, and it is. **You have to work for your reputation.** So, if you will care about your work, make quality your goal, and if you can act as a team player, you will become the 'guy (or girl) who can be counted upon'. It is a nice feeling to be respected and viewed this way, but it takes time, effort, and work.

<span class="textImportant">Become a person that others can count on.</span> Build your reputation, and you will be rewarded for it.

Also of importance, as mentioned above, is that not only quality of what you deliver matters here, but many aspects of teamwork as well, which is a topic covered in one of [the following sets of Elements](#elementsOfTeamwork).

<p class="backToToC"><a href="#listOfElements">&gt; back to the Elements' list</a></p>

## <a name="elementsOfVersatility"></a>Elements of Versatility

Versatility for software developers means adapting quickly and developing a range of skills to help them keep up with changes, as well as being able to put themselves in the bigger picture.

### <a name="element5SearchForAnswers"></a>Element 5 – Search for Answers

Often when you ask a teammate a question about a problem you are facing, they will just immediately type it into a search engine in their web browser. They don't know the answer, but they know where and how to look for it. A few seconds later they present to you a solution to your problem, taken from one of the first search results. You ask yourself: *why didn't I do that in the first place?*

**Most of the questions have already been asked**, and you will quickly find them on the Internet, along with proposed solutions. If this is what you do already, that's great, if not – give it a try. You will almost always find the solution in the very first few search results. It's just a matter of wording the query for the search engine in the right way, and it is something that takes practice, so don't be discouraged if the first few tries do not yield any relevant results.

You will often find what you are looking for on Stackoverflow, which has gained a lot of popularity in the last years. <span class="textImportant">If you find an answer on Stackoverflow, consider upvoting it to show its author that he has helped yet another fellow developer.</span>

At times, finding answers in the vast Internet might be hard, and it might require time and commitment. Keep in mind that <span class="textImportant">searching for answers is a <em>skill to learn</em></span>, and a very important one. It is also rewarding – it will quicken your development process and make you less dependable on getting help from other developers. What is more, <span class="textImportant">it saves time – both yours and your teammate's</span>, whom you would ask the question. Of course, it doesn't mean that you shouldn't ask for help when you are stuck with a problem – [Element 10 – Value Time of Other People by Asking the Question the Right Way](element10ValueTimeOfOtherPeopleByAskingTheQuestionTheRightWay) proposes a way for you to *help other people help you*.

<p class="backToToC"><a href="#listOfElements">&gt; back to the Elements' list</a></p>

### <a name="element6AcknowledgeTestingAsPartOfYourJob"></a>Element 6 – Acknowledge Testing as a Part of Your Job

Testing is vital in our line of work, and often there are dedicated testers on projects. They take care of testing once we assign a task to them that is, in our opinion, ready to go.

From time to time, though, tester from our team might be on holidays, get sick, or just have too many tasks on her or his plate to be able to finish all of the testing in time before the system goes live. It might also be a case that there just aren't any testers in your team.

Whatever the reason, you might be asked to help in testing. I often hear developers answer that *testing is not part of their job*. They sound like they feel offended by the notion of having to do some testing, like it is somehow going to diminish them, whereas, in fact, **testing is a part of every developer's daily work**. Whenever we write some code and produce a functionality, we should test our solution before it goes further down the workflow. I myself can't imagine claiming the task is ready, having not tested it myself, and asking tester from my team to take care of it.

Testing is rooted in the very concept of software development. If there is a chance to support the team by testing a couple of tasks in a time of need, why not do it? A little versatility goes a long way. Don't think about testing like something worse than writing the code, where <span class="textImportant">testing is in fact a part of the development process</span>.

<span class="textImportant">Help your team by doing some testing in a time of need.</span> Nothing wrong about it, and <span class="textImportant">having to test some of the other developer's work might just reveal to you how hard testing can get</span>. You can easily make it simpler for the testers if you provide information about the task you have done, covered by [Element 15 – Document Your Work and Provide Helping Information for Testers](element15DocumentYourWorkAndProvideHelpingInformationForTesters).

<p class="backToToC"><a href="#listOfElements">&gt; back to the Elements' list</a></p>

### <a name="element7LookAtTheBiggerPicture"></a>Element 7 – Look at the Bigger Picture

Imagine: a developer comes to work and there he is, with his tasks and problems to solve. He writes code all day and happily goes back home. That picture, for many of the developers I have worked with so far, would be a *dream job*. Unfortunately for them, it is not how the developer's work looks like most of the time.

There are meetings, supporting colleagues, code reviews, work time tracking, more meetings, tedious bug fixing, tasks time-requirement evaluation, business' needs analysis, and so on. <span class="textImportant">Our line of work consists of much more than just writing the code, and we need to be aware of that.</span> The workflow of delivering value is complicated, and varies from project to project, and team to team. What is important here is **understanding that there is much more to software development than... software development.** <span class="textImportant">Next few times when you'll be doing some task that is not related to writing source code, think how your work contributes to the overall process of software creation in the company that you are a part of.</span>

Two complaints that I hear from teammates very often are: logging work time and having to estimate time-cost of tasks. It can be tedious, but it is often necessary from your employer's point of view. He is, after all, paying you for what you do, and most probably there's a budget to consider, as well as requirements from stakeholders. Thus, knowing what the team has been working on and how much time it took is vital to the company. Same goes for the task estimation – knowing the cost of implementation of different business needs allows a better understanding of what can be delivered and when. Basing on that, your employer can choose, with the time-cost in mind, what is the most important and thus what should be the point of focus for the team.

<span class="textImportant">Whenever you join a team, become a member that contributes to the team's effort of delivering value.</span> Take a look at the bigger picture, and understand the project's and team's workflow. Keep in mind that your work consists of many different tasks. Writing source code is an important one on that list, though not the only one.

<p class="backToToC"><a href="#listOfElements">&gt; back to the Elements' list</a></p>

### <a name="element8EmbraceTheChallengeOfOtherTechnologies"></a>Element 8 – Embrace the Challenge of Other Technologies

Our world of software development evolves quickly, and many new trends, languages, frameworks, and technologies pop up every year. Each of us specializes in what she/he does and/or likes best, and we tend to stick to those same technologies for quite a long time. Sometimes we might be asked to do a task not related to our specialization. What should we do? Decline or happily try out something new?

It depends on what we are asked to do, which technologies are involved, and how much time it will take, and, possibly, how often similar tasks will pop up in the future. We have to evaluate all of those and make a choice. However, <span class="textImportant">consider that learning other technologies might be beneficial, and developers who are able to work with a broader range of languages and frameworks are valuable to employers.</span>

I have worked with developers who were very unhappy when they were asked to do something that was just outside their comfort zone. No one was asking them to totally abandon their language of choice, yet still they complained about doing something new to them. Instead of looking at it as a challenge and possibility to learn something new, they regarded it as a waste of time and something that was out of scope of their responsibilities.

Just to be clear, **by no means am I talking about leaving your favorite language and framework**, and starting working with other technologies that you have no interest in. What I mean is to be versatile enough to deal with tasks that might not be covered by your specialization, from time to time. If there are too many of them, then it is a good idea to talk to your manager about it.

<span class="textImportant">When asked to do some programming in a different language, or using a different technology or framework, try to look at it as both: a challenge and a possibility to learn something new.</span> You might like it, and if not, it might be an addition on your curriculum vitae. Getting basics in other technologies might be a huge advantage on the market.

<p class="backToToC"><a href="#listOfElements">&gt; back to the Elements' list</a></p>