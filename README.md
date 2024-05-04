# Management of exceptions

An exception is a problem that occurs during program execution. When an exception occurs, the normal flow of the program is disrupted and the program or application terminates abnormally.

In order to prevent such an unwanted termination, exceptions must be managed or handled and the necessary operations must be performed to fix the problem. Therefore, when an exception occurs, an object named Exception Object is created, which contains information about the type and time of the error in the program or application, then this object is provided to the system. From this point on, the system tries to find a way to fix the error. If the system finds a piece of code that can fix the error, it will be possible to reuse the system. Therefore, it is necessary to foresee the future in the parts of the program where there is a possibility of exceptions and to plan and write code to manage exceptions. The occurrence of an exception can have many reasons, some of the most important of which are:
- The user has entered invalid data.
- The program needs a file to run, which it cannot find and read its content.
- The connection with the network is interrupted or the memory of the device becomes unavailable.

Some of these scenarios occur due to user error, some due to programmer error, and some occur due to the lack of sufficient resources, or rather "physical resources". However, all these exceptions fall under the category of "technical errors". In addition to these errors, there are other groups of exceptions that occur due to non-fulfillment of Business Logic. For example, suppose an application is designed that allows users to shop online. Now, one of the users of this application wants to make a purchase, but does not have enough credit in his account. In this case, an exception condition occurs, which is not related to the technical aspects of the application, but the "business logic" of the application does not allow the user to perform a transaction with insufficient credit.

The point that must be observed about exceptions is that we must distinguish between technical and practical types of exceptions. With this, we will be able to use the general mechanisms of exception management in different programming languages and even use some software frameworks to manage exceptions, but in the case of practical exceptions, the user must Be aware of the exceptional conditions that have occurred and be ready to manage them, in which cases it is better to consider a separate exception or a distinct exception hierarchy to manage exceptions so that the user can manage them based on their own conditions. .

# Code reviews

One of the important recommendations that is always given to programming teams is to hold code review meetings. Many organizations and software companies place special emphasis on this issue and holding such meetings is included in their software development process regulations and has become an official administrative process, which the programming team requires them to do this. Such an emphasis indicates the importance and efficiency of these meetings. However, most of the programming teams do not want to participate in these meetings due to some issues. In this training, we are going to examine these problems and provide solutions to hold these meetings better. Programmers who have had a bad previous experience in this field often raise issues such as:

1- Some criticisms and opinions about the codes make the programmer feel that the critic only intends to ruin his image and has found an opportunity to attack his character and criticize his work.

2- Some critics, instead of examining important and fundamental issues, only emphasize the structure and arrangement of codes, such as the way of indentations.

3- In many cases, critics have not reviewed the codes before and enter the meeting without prior preparation.

4- Sometimes only one sample part of the codes is checked and other important parts are ignored.

5- Sometimes, the team will delay the code review until the main part of the code is complete, and then due to the large amount of information, the code review will be neither possible nor effective.

6- In some cases, because the members enter the meeting with the view that they are supposed to perform only one administrative task on the order of the manager, they do not pay much attention to the flow of the meeting and do not spend enough energy to advance it.

7- In some meetings, people who have nothing to do with the project are invited to the meeting, and this is a little worrying for the developers because they may express crude opinions!

Issues like this, plus many others, make developers unwilling to participate in these meetings. Therefore, programming teams should look for ways to solve these problems so that they can take advantage of it.

The first point that should be noted about review meetings is that the purpose of such meetings is not only to find errors in the codes, but these meetings should be aimed at sharing knowledge and awareness among team members and establishing common strategies. Coding will be held. Sharing code with other programmers gives people a sense of shared ownership of the code. In this way, everyone tries to work on the codes with others and instead of just looking for errors and mistakes, they try to understand the codes and find out their meaning and purpose, and to advance and improve them. to cooperate

During the review session, try to remain calm and express your opinions gently and maintain the respect of others. Make sure your criticisms are constructive, not sarcastic and just meant to poke fun at others. Recognize the different roles in the review meeting so that you do not allow, for example, the opinion of the group manager to influence the opinions of others or prevent the truth from being told simply because he has a higher organizational position than others. For example, one type of role division can be such that one member focuses on documentation, another on exceptions, and the third person on functions and usability of codes. This method helps to ensure that all group members are responsible for the review and that all the participants of the meeting are active.

Review codes regularly every week. Spend a few hours of your time attending these meetings. Select reviewers in rotation. Allow new team members to participate actively in these meetings. Maybe they have little work experience, however, because these people often just graduated from university and have new knowledge and awareness, they can create a different perspective in the group. Of course, the presence of professional and expert members is also necessary so that they can transfer their unique knowledge and experience to others. Such people can find error-prone codes more quickly and accurately than others.

If all the code written by the programming team follows defined conventions and standards that can be controlled with certain tools, the flow of code review and review will be easier and faster, and in this way, the team in The review session does not waste its time on formatting and formatting the codes.

Perhaps the most important thing that helps teams to reap the benefits of such meetings is to turn a boring and boring meeting into a lively and fun one. If the members of the meeting feel that their position is threatened, it is difficult to motivate them to participate in the next meetings. Code review meetings should be held informally with the main purpose of transferring knowledge and information among members. Everyone should try to create a friendly and stress-free atmosphere instead of sarcastic and provocative comments. Be sure that holding meetings in such an environment will improve the quality of the codes, ensure compliance with standards, and as a valuable educational tool, it will increase the knowledge and experience of developers.

# Write your programs in the language of customers!

As a programmer, the owners of various industries and businesses will probably approach you and order you work. To carry out these orders that are related to the work processes of customers, you can model those processes using the capabilities of different programming languages. For example, the owner of a store may order you a program to control the goods in the store's warehouse. Therefore, you should model a warehouse in which purchased and stored goods are recorded and their status can be tracked until they are available in the warehouse. Our advice to you is to write your program in the language of the ordering customer in these cases.

The purpose of writing your custom program in the language of the client is to use the terms of the client's business in the program codes and to implement his relationships and working procedures in the program. Let us clarify the matter with examples. Consider the example of a store. To model purchased items, we need to define a variable to store the name of the new item to be used later in other parts of the program. We know that we need a name to define any variable in programming. The best thing to do is to choose a name that represents what is supposed to be stored in the variable, and at the same time is known to the client, instead of using a meaningless name such as x. For example, let's name this variable new_product_name and store it in this variable with the arrival of each new product.
```
new_product_name = "gjg"
//or
new_product_name = "fa"
```
Do the same for procedures. For example, it is not the case that the warehouse staff keep all the purchased items in one section, but they store them in different sections according to the type of product. Perishable food in the cold room, creams in the hygiene department, fabrics in the textile department, etc. . . When it's your turn to model this procedure, you might think to yourself that placing items like food, toiletries, etc. together in this virtual model won't affect them. Therefore, instead of spending more time and writing more codes, to put the names of these products in separate tables in the database, you decide to put them all in one table so that when you want to know the status of a product Check that the program codes do not search one table more in the database instead of several database tables. This may be convenient for you, but keep in mind that this app is for the store owner, not you!

It's best if your code explicitly simulates storage procedures in the warehouse. The advantage of this type of explicit coding and in accordance with the client's work routines is that, firstly, it makes it easier for you to correct errors and changes needed in the program (even if you forget how each piece of your code works and for what purpose). (slowly, you can refer to the client's work procedures and decipher its algorithm) Second, if another programmer replaces you to update the existing system, through familiarity with these work procedures, he will understand the meaning of your codes. He understands easily and he doesn't need to refer to you to interpret them or to rewrite a new program that he can understand!


# Make your designs perfect

In this article, we are going to talk about one of the current crises in the world of programming and software design. With the advancement of technology and the increasing dependence of people and industries on computers, the community of programmers has faced an increasing demand for the design of application software. Naturally, programmers who can write their codes faster and respond to the needs of more customers will benefit more from this market; But the speed of doing things has become a problem, and we have to see at what cost this increase in speed.

Remember that coding is a creative work and the programmer creates a new design in every project. Therefore, in order to create a high-quality and reliable plan, planning should be done in advance, all aspects of the plan should be carefully examined, the best tools that can be used to implement the plan should be provided, and finally, all capabilities should be carefully considered. and facilities to be used and after finishing the work, test the designed software from different aspects to fix all its bugs and defects. But the crisis that the world of software design is facing is that many programmers ignore these procedures for the reason mentioned above to increase speed.

Some programmers immediately start coding after accepting any project, without having a specific plan in mind. In writing each piece of the program, they think about which command can move the work forward. Regardless of whether the written codes are of the necessary quality and beauty, and if they can achieve the customer's desire to some extent, they continue to work and only think about changing the codes when they encounter a problem. do

In fact, in these cases, the programmer uses the most accessible features of the programming language of his choice to organize his work and quickly deliver it to the customer. Customers, who often don't know anything about software design, only pay attention to the speed of the work, and at the end of the work, they inevitably end up with incomplete and incomplete results!

Maybe these types of activities can be beneficial for programmers in the short term, but you should know that in the long run, they distinguish professional programmers from non-professional programmers. So try to create lasting and reliable designs. Your client may not use some of the software's features for a while and as a result may not notice its possible defects, but it is your duty to check your software carefully.

You should know that the design of a software is not complete unless you test its quality from various aspects and control its performance when it is published. Advanced design languages and techniques will greatly help you to create complete and flawless designs and know the truth that regardless of code, great and great designs are created by great programmers who dedicate themselves to it. They are experts in their profession!


# Pay attention to the layout of the codes!

If you have the experience of coding relatively large programs, you must have noticed that instead of writing new codes, you spent most of your time reviewing previous codes to make the necessary changes and fix their bugs. . One of the important factors that determine your speed and efficiency in code review is the code layout. A good layout with the correct indentation and the right amount of white space makes a huge difference in the time it takes to look at the commands in a code and understand what they mean. In this tutorial, we are going to propose ways to optimize the layout and arrangement of codes.

Simplify code scanning:
Let's say your team has written a program that has several different classes. When running program classes, it does not matter to the compiler whether public elements or private elements are defined first in the body of the class, or whether constants or fields or methods are defined first; In other words, the order of the components of a class doesn't matter to the compiler, but what about you?

You should be aware that people are often good at adapting visual patterns, so one approach you can follow to make your code review easier is to define a pattern for placing application elements in your code, and have all team members When coding different parts of the program, follow that pattern. As an example, we can take the PHP programming language as an example. A site called php-fig.org has designed a standard called PSR, which stands for PHP Standard Recommendation, for PHP programmers. By using these standards, those interested can benefit from codes that other PHP programmers look at. They will be less confused by their codes

To clarify this issue, we will give some examples from other programming languages. Most C++ programmers first put the definition of public methods in the body of their codes and below them the private methods, while this procedure is completely opposite in coding in C# language. Of course, note that we get these patterns experimentally from the teacher's resources when learning any language and follow them unintentionally, and following them makes other programmers easily read our codes, with Now you can define a special standard for yourself so that all team members follow it.

Arrange the code so that it conveys the meaning of the code:
One of the recommendations that programmers are always given is that when naming classes, variables, methods, and other program elements, use meaningful names that indicate as much as possible what each program element does. . You should know that the arrangement of the codes should also be such that the purpose of the codes is clearly defined as much as possible. If you write your code in a simple text editor, the trouble of setting up its layout is on you, but today most programmers use integrated development environments (IDE) like Eclipse, which can automatically arrange the layout. Determine the codes. However, our advice to you is to always keep in mind that these tools cannot understand what you mean by the code you have written, so sometimes you need to manually make changes to the code layout to understand what you mean. make it clear

Compress your layout as much as possible:
Most programmers enter each command in a separate line when they code in a development environment, as far as we can see, most of the commands do not even continue to the end of the line, so at the end of a program with There are many lines of code and countless empty spaces. However, you should know that the best approach is to compress your layout - to the extent that it does not harm the readability of the codes. The advantage of this work is that it becomes easier and faster to move between codes (especially in large programs), or for example, in web applications, the amount of data sent from the server to the clients, or the time Reduces page loading.

# Getting to know communication skills and learning foreign languages

One of the integral parts of the coding profession is communication; Although a significant part of developers' time is spent interacting with computers, compilers, software development tools, and most importantly, the project they are working on, developers sometimes have to communicate with others for various reasons.

The success of large and important programming projects nowadays requires more than technical reasons, it requires the existence of constructive interaction in a group-social manner; Many successful programmers are those who, in addition to mastering one or more programming languages, also master communication skills and other living languages of the world besides their mother tongue.

There is no need to explain that in the process of coding, the developer speaks through the codes he writes and asks the system to perform the tasks he wants. A good programmer in interacting with other people also knows very well with what language and in what way to interact with them so that he can convey his meaning to others in the best possible way and create an effective communication.

Another point that should be considered in the field of personal communication in the field of software development is that, apart from developers, many stakeholders are involved in a relatively large software project, including the product manager, project manager, user experience expert, The marketing manager, software testers, front-end developers and also the main product owner (customer) mentioned that some of them have technical knowledge and others don't.

A good developer is someone who is well acquainted with the needs of each of the above-mentioned people and understands them well, and to achieve such importance, we must be able to speak with each of the above people in their own language; In other words, sometimes we need to speak technically and sometimes we have to express our meaning in the most non-technical way possible so that the audience fully understands what we mean.

Let us use an example to clarify this issue; Suppose we have a client who is an accountant and we are going to write a financial software for him; In order to verbally communicate with this customer in the best possible way, we must be familiar with some accounting concepts such as balance sheet, debtor, creditor, financial statement, current assets, cost principle, debt, arrears, etc. Jargon items are said.

Jargon refers to the specialized terms of any profession that a significant part of the conversations of people active in that field are made using these specialized terms; For example, different people such as doctors, lawyers, accountants, mechanics, programmers and other specialists each have their own work terms that they use easily while talking to their colleagues and both parties understand each other's meaning well.
In general, when a programmer has the task of translating the needs, ideas and concerns of customers into code, familiarity with these jargons is a necessity. Also, apart from all these topics and knowing that communication and social skills are an integral part of a developer's life, having knowledge of English is a must for a developer who plans to label himself as a professional.

In other words, a developer who wants to keep up with the world's software knowledge, easily read the documents of programming languages, libraries, etc., easily search on Google and Stackoverflow and communicate with other developers around the world, having English language skills (at least reading and writing) is the least expected of him.

In other words, if you are a novice developer who is planning to choose software development as your main job and source of income, but you don't have enough knowledge in the field of English, it is recommended to stop learning your programming language and start learning English because then From mastering the skills of reading and writing - and of course speaking and listening skills if possible - the speed of your learning and progress in the field of coding will be much faster than when you did not know the language!

# Getting to know the concept of refactoring in coding

One of the things that most programmers come across is a concept called Refactor, which means rewriting the code that has already been written. There is no need to explain, the experiences that a programmer gets after a few years of coding are not comparable to when he just started working, and surely after a few mornings when he looks at his codes, he will be upset with his coding style. And he decides to refactor his written codes. In this part of the tutorial, we are going to see when is the right time to rewrite the previous code, and if we know why and how to do it, our time will be saved significantly.

Before you start rewriting your code, be sure to consider the following: One of the best approaches to whether or not to rewrite your code is always to test your code using the tests you need to test it. Let's write tests, because by doing this, we will understand the strengths and weaknesses of our program, and when we want to refactor the code, we will not tamper with the parts of the code that are working well, but at the same time, we will fix the weak points. we will do Programmers always think that they can write code that works better than the current code, and this is the mistake that should be avoided as much as possible.

Warning In addition, you must resist the temptation to rewrite any source code. Always remember that we should use previous codes as much as possible even if the codes are not cleanly written! When we delete previous code, it means we waste months or years of effort and coding.

In the code rewriting process, applying several small structural changes is much better than one major change. In other words, small changes allow you to more easily test the effect of those changes on your application and see their feedback.

After completing each module - or rather, each part of the program - our source code must pass several tests. As soon as you make a new change in your code, be sure to write tests for those changes. In fact, these tests have a function like End User, as if it is working with our program, and they ensure that the software that will reach the customer is bug-free. In addition, never delete old software tests, because you may have had a specific idea in mind in the past months, and you wrote a unit test to test it, but now that you are rewriting the code, your thoughts are completely directed towards And it has not gone towards that particular idea.

Try not to include personal preferences in coding as much as possible. If a piece of code is working properly, there is no need to rewrite it at all. If the code you wrote isn't clean, that's not a good reason to rewrite it at all. If the code in front of you is inherited from another programmer, there is a high possibility that you think that your code will be much better than the previous programming, which is not a valid reason at all!

Using new technologies is not a good reason for refactoring. One of the worst reasons that a programmer can give for rewriting the codes is that the program codes are related to the technologies of several years ago, and now the version of the software and programming languages used in that particular program have been greatly improved. In such cases, you should definitely check the framework or programming language in question to see if its new versions are really improved or not. If they really help to improve the performance, maintainability and efficiency of the software, the code should be rewritten, otherwise the code should be left as it is. In the end, always remember that people are always prone to make mistakes. Rewriting the code does not mean that the new code will work better than the old code or as well as the old code!

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
