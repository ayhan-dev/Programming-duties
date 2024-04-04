
# Reuse your previous codes in appropriate situations

Many professional software developers are used to writing reusable code. The existence of reusability in a piece of code allows us to use it in coding several different programs. When we say that professional programmers include such functionality in their code, we are saying that this is a positive thing, however, this issue should be carefully examined and see if this is correct under all circumstances. ?

Is the reuse of codes always approved under any circumstances? To answer this question, we need to find out the advantages and disadvantages of such work and then choose one between reusing the already written codes and writing new codes by making the conditions light and heavy. Therefore, in this tutorial, we are going to talk about the advantages and disadvantages of reusing codes.

Advantages
Code reuse reduces coding time, which will reduce the costs of a programming project. Suppose you or another programming team worked on a problem and found an optimal answer for it, and now this answer is available to you. So there is no reason why you would want to search again for an answer to a solved problem.

Reusing previously written and tested codes will greatly reduce the amount of possible program bugs. In general, the more lines of code written in a program, the more likely that there will be errors among those codes. When a piece of code is used in several different programs, that common part is tested over and over again in all programs, and the possibility of errors in it is reduced.

Usually, reusable codes are divided into separate software libraries, so that any programmer can use these ready-made libraries according to their needs. The advantage of this work is that every programmer can code according to his strengths in a specific field. For example, security specialists can work on codes related to this field and share them with other programmers by producing powerful software libraries in the field of security, while, for example, UI specialists work on related issues. They focus on designing and optimizing user interfaces. Reusing codes appropriately and efficiently can help avoid unnecessary repetitions and redundant commands.

Disadvantages
Despite all the advantages that reuse of codes has for us, depending on different conditions, it is possible that this work is not only not useful for us, but also harms the program.

Suppose we use a library of codes in several different parts of the program. This causes the code dependencies of these sections to increase. If we want to change or modify the common codes of some of these parts, we must be careful how this will affect other parts.

It's possible that the library or framework you want to reuse in your application will be slower than expected, depending on the programming language or platform you're working on.

If you use code that has already been written by other programmers, there will be security and reliability issues and usage permissions issues. In addition, the evaluation of these codes usually takes time and it is possible that you will notice weaknesses in the design and bugs of those codes after a long time.

Managing code that is shared between different programs can create additional costs for the program. In addition, sometimes implementing and synchronizing these codes with your own code is too time consuming and requires a lot of work. However, as a programmer you have to find the skill to consider all aspects and choose whether you want to reinvent the wheel, or reuse it with a little modification and adaptation to your source code. do.


# Technical Debt

It often comes down to choosing between "doing a project properly" and "doing a project quickly," with speeding up the design process of a project seeming more attractive initially, arguing that later on, you can always go back to the code and fix any problems! However, experience has shown that when the word "later" arrives, it brings along with it numerous bugs and issues that the programmer must focus more on, leaving behind past - albeit minor - problems.

This policy in programming is known as Technical Debt, which can be literally translated as "Technical Debt" (be sure to note that the letter "b" is not pronounced in the English word "Debt"!). Technical debt is not a good thing at all and sometimes leads to disasters in software development. To clarify this issue, let's provide an example. Technical debt is like taking a loan that gets our work going in the short term but unaware that in the future, we'll have to pay back our loan with an interest rate - say 30% more - (by the way, they say in some non-Muslim countries the interest rate is around one or two percent, while in our Islamic Iran, it sometimes reaches fifty percent. Are they Muslims or are we? Let's move on!)

In programming, the situation is exactly the same. Although sometimes we can use solutions to speed up our coding, this makes adding new features to the project difficult in the future, and in other words, we can't easily refactor our code. Interestingly, as time passes and these problems accumulate, finding solutions for them becomes even more difficult. But if we're behind schedule on our project and forced to prioritize speed over quality, what then? Our recommendation is never to sacrifice the quality of work for the sake of speeding it up, but if you really have to, then do it, but always remember that you've created technical debt for yourself, which you must pay off at the earliest opportunity. Also, make sure to mention this issue in the project documentation so that it doesn't get forgotten, as otherwise, you may end up paying a hefty price for it.



# Functional Programming

Functional programming has gained many fans in the last few years. This paradigm is the way in which the logic used in the program is considered as mathematical functions. A correct understanding of this type of paradigm will significantly help to improve the quality of the code that is written, and if you - as a programmer - use the principles of functional programming, the quality of the program that you write will double, which will eventually increase with the number of Fewer lines of code will get you the result you need.

When we use functions in our projects, specific responsibilities can be assigned to each function, and functions can provide different outputs to other parts of the program using the arguments they receive. Programs in which functions are used correctly are easier to debug than traditional programming methods. Functional programming has worked well in object-oriented programming, but this paradigm cannot be used in all situations.

# Simple is beautiful

There is a sentence of Plato with the theme that "harmony, external beauty, elegance and balance all depend on simplicity." And if this sentence is used by programmers, it will have many benefits for them, including more readability of codes, easier maintenance of scripts, increased coding speed, and finally higher quality of written codes. All these things - and even more things - are not possible except by applying this view of Plato, that is, simplicity.

Now we have to answer the question of what kind of code the beautiful adjective refers to. This question is very abstract because the concept of beauty is something completely relative. Artists' understanding of beauty is far different from that of engineers or programmers. Therefore, it is necessary to solve the problem of beauty in programming a little!

To understand this better, it is better to visit GitHub and see some scripts written by programmers from different parts of the world. By comparing different codes, you will notice that there are some programmers who follow a set of rules well, and this issue leads to the code written by them looking more beautiful. It is interesting to know that the simpler the code, the more beautiful it looks. Although there are some programs that are very complex and do strange things that make people wonder, but if we divide these programs into smaller parts, we will see that if the programmer of that program was a professional and Simplicity has faith in coding, the small parts of the program are completely simple and understandable, each module has a specific task, different parts such as classes, methods and variables are well named so that if other programmers look at the source code , they will easily understand the task of each part of the code. In short, beautiful code is code that is simple. Different parts of the software should have simple relationships with other parts and be easy to understand.

# Observe cleanliness!

There are certain people who, when they see garbage on the ground, regardless of who threw it on the ground, they pick up the garbage and throw it in a special place (of course, this is more common in first world countries). In other words, such benevolent people prepare a clean space for other people who will be present in that environment. There is a saying that goes "Make the world a better place for future generations than what was handed to you."

A good programmer is someone who, when he takes over the code of another programmer - no matter who the previous programmer was - he will do his best to improve the code, while this improvement works. It can be in the field of improving code efficiency or even in the field of commenting. What do you think will be the final result in such a situation?

It seems that if the programmers follow such an approach, the quality of the codes that are written will increase day by day until the presence of bugs in the codes will become an abstract matter. Now this question may arise for you, what if the previous programmer was instead of a code writer? In response to such a question, it should be said that you don't need to improve all parts of the code, but you just need to do everything you can, or at least try to clean the codes you add to the previous module. Write regularly. This clean writing of codes can end with the correct naming of functions and variables, compliance with spaces, etc.

In programming teams, after adopting an approach like the one mentioned above, an atmosphere should be created that even if one team member wants to do messy coding, he will be embarrassed by the other team members and correct himself, just like Situations that happen at a fancy party: Does someone throw cucumber skins on the parquet after eating them? Never!

# Choose the right tool

Many of the software and applications that we see today and have achieved relatively good success, their coding was never started from scratch, but such software was developed using existing tools - here we mean the tools of components, libraries, frameworks. and... are made. In this regard, when we intend to start a project, we must choose the most appropriate tools for our project, and the bigger our project, the greater the need for research in this field.

Regarding the reasons why some projects are not coded from scratch and use existing components and libraries, the following can be mentioned:

1- Software and applications grow over time, become more complex and eventually become more professional compared to their beta version, while the time allocated for the development of such software and applications becomes more and more limited. . It seems more logical if programmers spend more time on coding the infrastructure of the project (which is somewhat similar in most projects), to focus on coding specific parts of their project.

2- The components and frameworks that are used all over the world have far less bugs than the code that a freelance programmer writes in his office!

3- Many frameworks available in the market are provided to developers for free, and the same issue indicates that the costs related to the development of a project will be greatly reduced.

4- The development of the project infrastructure in various fields such as security, efficiency, etc. is a sensitive, precise, time-consuming and costly task, but if you use free and open source components, you can ensure the timely and structural update of your project. do.

keep in mind
It should be noted that the Facebook company first used PHP programming language to program this social network, but after this network opened its place among users and achieved huge revenue generation, the managers of this company decided to use a proprietary language. They developed this company under the name of Hack and built the Facebook social network on it.

What is certain is that choosing a combination of available tools for application development is a sensitive task and requires experience in this field. For this purpose, we have brought you the following solutions that can help you choose the tool you want:

*- Each tool will have the best effectiveness in a specific platform. What we mean here by the platform is the database structure, communication protocols, server, web service, API, etc., so there is a possibility that the tool you have chosen is not compatible with your software development platform, and this problem leads to Your project will become more complex.

*- The tools that we see today have a certain lifespan, and when an update for them is released to the market or a new version of them is available to developers, it is possible - if not necessarily so - to see many changes compared to the version Let's face it, sometimes new versions of a specific tool - for example, a programming framework - have many structural changes compared to the previous version, which makes them completely incomparable. For example, the Laravel web programming framework has completely changed the structure of this framework in version 5, and this is the case if you have been using version 4 of this framework and now you intend to migrate to the latest version. , your whole project will be changed (note that the more frameworks and tools used in our project, the deeper this disaster will be!)

*- Some of the available tools require configuration or adjustment, which may require spending considerable time and money.

*- Some of the so-called free tools are not free as they should be. At first, we think that the tool in question is completely free and we start using it, but when the project reaches its critical points and requires the use of certain components, it will be discovered that part of the source code must be modified. buy from the original developer and this issue can overshadow the future of our software.

*- Some tools create limitations for us after developing the software with them. For example, there are some software licenses that require the developers who use them to publish their software and its source code in a completely open and free way, which such a restriction will certainly not be pleasant for many developers!

What is certain is that you will be the final decision maker, so you should develop as much as possible the codes that are related to the project infrastructure using the best available tools or frameworks and code the codes related to the specific module of your project personally.

# What is the user's need?

All those who program think that the users of the program or application they develop think like them and they believe that other users will have the same relationship that they have with their program, which is a very wrong idea. Such a belief is called False Consensus Bias from the point of view of psychology. It is interesting to know that when users interact with the program written by us in a way that is contrary to our expectations, we label them "a non-professional user"! But this is if we are non-professional programmers who have not identified the needs of our target community very well!

What is certain is that users never think like programmers because, unlike developers, they sit at the computer for less time, they are not very familiar with how systems work, they lack the problem solving skills that most programmers have. They are not familiar with the patterns that programmers use to design and code, etc. In other words, the relationship that an End User has with a program or application is like the relationship that a programmer has with a car. It is true that the programmer knows how to get into the car, fasten his seat belt, etc., but the programmer never knows how the system of this car works.

To solve this problem, we should ask a normal user to interact with our program, site or application and carefully examine how he communicates with the software. In fact, we should see what the needs of this user are, where he encounters problems, in which parts he gets confused, etc. We will give an example to clarify this issue. When a programmer, for example, codes a site, when he encounters a problem in the user area, he knows for sure how to fix that problem, but this issue does not apply to normal users, and they may As soon as they encounter the smallest problem, they give up their goal. Another thing we should always keep in mind is that most of the time there is a gap between what users really need and what they say. In other words, according to the words of the late Steve Jobs, it is not the users who say what they want, but it is you as a designer who should understand the needs of the users and present them to them in the best way.

To solve this problem, instead of listening to the users, we should look at their interaction with the site, software or application and assess their needs based on their behavior with our program. In a word, if we look at the behavior of a user with our application for a few minutes, it will be much more productive than conducting a few hours of interview with several potential audience about their needs.


## Always be learning new things

Our life in the age of technology is very exciting and interesting. Technologies are growing rapidly and news of new innovations and achievements in the field of science and technology are published every day. On the other hand, we see that the growth of technology has had a great impact on learning processes; For example, the Internet has provided a platform that enables users to access a huge network of information and learn about new innovations.

This high speed of scientific growth and easier access to scientific resources has increased the number of job competitors, especially among programmers. What is more important than anything else is that we notice these changes and developments and know that in order to continue working and compete with other programmers who are active in the programming market, it is necessary to constantly update our knowledge. Let's update it, otherwise one day our knowledge will become so old that it won't be used anywhere.

If we come to believe that no matter how professional we are in our work today, in the near future this level of knowledge and skill will be very little and will not create a competitive advantage for us compared to other programmers, then we should look for a way. Do things to increase your knowledge and skills. Fortunately, some employers, in order to support their human resources and help their business by spending money and time, conduct training courses and raise the scientific and skill level of their workforce. However, you may not have the chance to work with such teams and you have to find a way to learn new things yourself.

Here we are going to introduce you some practical methods and useful resources so that you can use them to increase your level of knowledge and skill as a programmer. The list of these suggestions is as follows:

1- Read books and magazines, visit blog posts, sites, and Twitter feeds that review news and new topics in the field of software and IT. Try to stay in touch with a community of programmers.

2- If you really want to get to know a new technology, get your hands dirty with it! Start coding. Try to master them by trying new software.

3- Always try to work with those who know more than you, because working with smarter and more experienced people and their supervision of your work creates the motivation to learn both in you and in Interacting with them, you can learn many lessons and gain useful information. When you are alone with people who have a lower level than you, you lose both your competitive motivation to learn and the fact that you probably have to spend all your time teaching them, which somehow prevents you from learning new topics. will be.

4- Use the help of virtual mentors. There are well-known people in the web space who are great writers and developers. Follow their activities and writings on their websites and blogs. Many of these people answer other people's questions and you can use the guidance of such people who may even live on another continent virtually.

5- Start learning the frameworks and libraries that you use. Knowing the exact way something works will help you understand how you can make better use of it. If they are open source, then luck is with you. Search their source code, because they are written by intelligent and experienced people, and reading them will give you a better view and inspire new ideas in your mind. Try to see the source code of well-designed sites to get to know how they are designed.

6- When you make a mistake, encounter a bug in your code, or encounter a problem in coding your program, try to understand what really happened. Someone may have faced such a problem before you and after finding a solution, shared it on the internet. In these cases, searching on Google - as well as searching on the Stack Overflow site - will help you a lot. Also, try to share your findings with others.

7- According to a satirist: "Those who have complete mastery of a subject use it and work with it, and those who do not know anything about it teach the same subject!" The fact is that one of the ways to learn a subject is to teach it and talk about it. When some people are going to be your audience and ask you a question about something, it will create a lot of motivation for you to learn. Try to get information about new topics and technologies and share this information with friends and colleagues.

8- Choose a topic that you are interested in and try to study it collectively with a group of people. Be sure that by cooperating with others and using their opinions and experiences, the impact of this collective learning is far more than individual learning. Fortunately, with the emergence of wide social networks, these activities can be done in a team format and virtually.

9- Participating in conferences is also a good option to learn about new findings and scientific topics. Even if you are not able to physically attend such conferences and seminars, you can follow many of them online without paying any fees.

10- Have you ever used program code analysis tools, or paid attention to the warning messages of the development environment in which you code? A good way to learn is to understand what they are saying and why they have such analysis on your code.

11- Follow the advice of professional programmers who say to learn a new programming language every year. Get to know at least one new tool or technology and learn how to use it. Knowledge about new technologies will give you new ideas for better use of current technologies.

12- These days, everyone knows that just learning programming languages or knowing how to use new technologies will not give you a competitive advantage. You must be familiar with the field in which you work to be able to understand the needs of your customers. Knowing how to work more effectively and have a more productive role in the work environment will also be useful. For example, these days most companies are looking for programmers who are familiar with Agile methods in addition to coding skills.

13- If you are one of those who lose a large part of their time in commuting and city traffic, you can save this time by listening to audio files and educational podcasts that are widely available on the Internet. Turn wasted time into a good opportunity to learn and gain new information.

14- It might not be bad to think about continuing your studies at the university. Although many people believe that the country's universities do not have a good yield and their output is not programmers who are ready to enter the job market, nevertheless, you should know that first of all, university classes definitely create a solid scientific foundation for your knowledge. Secondly, each of us can greatly contribute to the dynamics of student environments and bring industry and university closer with our motivation and interest.

In any case, technology is changing rapidly and if we want to stay behind this caravan, we must devote time to learning new knowledge and information along with work. No matter how little this time is, even a few hours a week, it can produce useful results.
