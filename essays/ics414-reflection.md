---
layout: essay
type: essay
title: "Still in beta: My reflections and growth in ICS 414"
# All dates must be YYYY-MM-DD format!
date: 2025-5-16
published: true
labels:
  - Software design
  - Learning/Reflection
---
<div style="text-align: center;">
  <img 
    src="../img/Screenshot 2025-05-15 222331.png" 
    width="1000" 
    class="rounded" 
    alt="spire login picture" 
    style="display: block; margin: 0 auto 50px auto"
  >
</div> 
  Now that the semester is coming to an end, I think that now of all times would be the perfect time to share some of my thought process, failures and successes, and my overall experience from this class. It's been a very insightful experience, showing me a lot about myself, what some of my weaknesses are,
  and what the most important takeaway for this class was. While not very satisfied or pleased with my own performance in the class, which was completely all on my end, I believe that I could've done a lot of things better, not just software related but through team communication, time management, and overall
  responsibility. But before that, I think it would be best to sort of explain this whole story from the beginning:

## ICS 314 part 2?
  Having just finished ICS 314 last semester, when I saw this class available for this semester I was very intrigued, questioning whether or not I should take it. I had some pretty rough turns during ICS 314, mostly due to poor preparation and discipline, but nevertheless, having 
  heard a lot from my ICS 314 professor about how much more in depth this class was, I made up my mind and decided to enroll. When first walking into the classroom for the first time, I was completely just expecting a vaguely reminiscent experience of ICS 314: more framework/template practice, 
  more WOD's, etc. But as soon as I sat down, me and the whole class were met with a pretty shocking revelation: no quizzes, no lectures, no homeworks, and crazily enough, no WODs! Only one thing was due this semester, that being... a single project, specifically a financial analysis application for a company called Spire Hawaii (A real client!). I think most of us were pretty taken aback by that, 
  but to me it sounded actually pretty promising. As Professor Moore had told us, this was essentially (almost) a freebie A: stay consistent, and you'll pass. However, for me, I knew I would have to really push through and keep myself on task to really get through this. No week by week WOD's to 
  atleast force me to slightly study, just pure, independent responsibility. After the first couple days, we eventually had to form teams, similar to the end of last semesters ICS 314 class where we also had to develop a project, with my fellow team members being Adam, Alyssa, Xing, Kenneth, Robert, 
  Ana (who unfortunately left later on), and myself. I knew that there was a whole lot more I'd have to learn for this class, and I was originally pretty excited to learn a bit more about how we were gonna tackle this project. 

## Back to the past
  With the majority of my team members having been out of ICS 314 for a while now, I was pretty much the noob in the group. Having realized that my ICS 314 class was the first to switch to a new tech stack (postgreSQL for databases and next.js for app development), and that majority of the people there werent fresh out of ICS 314, I quickly realized I was in the minority
  for the vote. However, I never really voiced against using Meteor and MongoDB (the old tech stack), as why should I inconvenience my whole team of 7 people to learn the new tech stack when it could just be me doing the switch? It would be way more comfortable (and efficient) for the team to work with something they're familiar with,
  so I just decided I had to suck it up and experiment with the meteor app template we were provided. After looking up the documentation, it seemed pretty similar to the nextjs app template: similar compiling and run commands, etc. However, the biggest difference was in the file directory structure and overall app function: different routing style, schema validations,
  tags, even the user account and password tokenization was different as well. I got pretty nervous as I basically thought, "I gotta teach myself essentially what I learned in the latter portion of ICS 314 within these first few days". It actually went pretty smoothly, as I just sort of looked at the content of what my teammates were committing,
  adding pages, user roles, and just sort of worked out the file dependency, structure, and organization for myself. It was a pretty good test to see how much I could learn about this new environment and I'm pretty pleased with it. However, little did I know that code development-specific problems were the least of my worries...

## A lesson in finance: Tables, graphs, and more tables
  As our main goal was to make an application that could confidently display, modify, and assess certain financial information (primarily business related costs and also relevant generated forecasts from current financial data), and also since the majority of the placeholder for this that the company was using were very large, complex excel spreadsheets, we knew we had two main objectives here: 
  * Learn how this mass of excel sheets works, and...
  * ...implement it through code.

  I can testify it was an intimidating monstrosity of a spreadsheet, with a ton of financial data, formulas, theoretical scenarios and forecasts (percentage or multiplier based modifiers that could affect multiple years and rows of financial information, which we'd have to implement into the app). Thinking about it all at once was pretty scary, so the best directive we decided on was to split the problem up into smaller parts,
  something pretty similar to (essentially the same as) Agile project management, which was a concept learned from ICS 314 to help streamline and efficiently progress in our team management and development progress, with the main pillars being:
  1. Split the project into milestones, which themselves consist of smaller, bite sized tasks
  2. Further split the tasks into different issues on the GitHub board, where each team member assigns themselves multiple (around 1-2 per person per milestone)
  3. Code reviews, to see how we can improve our programming skills and also learn from past mistakes or habits
  It was a pretty solid approach that could be applied to a majority of problems (not just development), and so we sort of went with it.

### The first stretch
  From the start, we sort of knew how some of the work was going to be split up: Adam and Alyssa generally seemed pretty confident and capable, so they were doing some of the role stuff, and Financial compilation data, and getting the database set up. I was sort of down to make the graph visualizations and also different stress test vs. forecast functions for it, where different rows of financial data could be plotted and compared against each   other. Kenneth was mostly doing some of the workpaper editing for the different financial data rows, Xing handled the stress test functionality, Robert worked on the overall website function, github setup, and some of the workpaper stuff aswell, and Ana I think was also helping implement the Financial compilation data. I was pretty interested in implementing a graph, as it was something that I had never done before, and having chosen chartjs to display the graphs, it was pretty interesting reading up on how it worked, data parsing, etc. I got it working pretty fast and was excited to implement more functionality, like plotting different stress test variables against each other, different value/row selection plotting and comparison, etc. However, I think from here on was where our momentum sort of started to breakdown a little bit. As I said before, I never doubted the capabilities of anyone on our team (I was most definitely the least capable in technical capacity and experience) and I knew the people I was working with were very smart and able, but I had a feeling that there was going to be some form of communication difficulties and turbulence along the way, as is one of the most difficult things to overcome in team coordination.

### Hitting roadblocks and navigating team challenges
  As the milestones went on, I felt that although we had, in our team contract, agreed to do occasional discord meetings, I feel that communication for our team was definitely a weakpoint. There wasn't much talking in the discord about how we were doing with our tasks, any problems we had, etc. I was really impressed with Adam and Alyssa, as in my opinion, they definitely took most of the initiative for communication, with Alyssa always making the code review issues for us to fill out. However, as nothing related to project development itself was addressed, I feel like many dependent factors and issues in the project started to stack. Primarily, we didn't have fundamental financial compilation data until nearly 2-3 months into the semester, and most of the actual functionality of the application heavily relied on that, with most of us creating our functionalities with placeholder data. We also didn't get the database up and running or even discussed it until pretty much the end of the semester, with Adam doing it almost solo. I feel guilty for not having attempted to touch ground with them and atleast reach out or attempted to communicate, as it possibly could've made a significant change in our project's devlopment trajectory; maybe we could've gotten the database up earlier if I had said something, which would've motivated me to learn more about MongoDB collections, and how I could get them to work with my graphs and properly organize and parse that data and display it on the graph. From this, I learned a really, really important lesson: My motivation and excitement for contributing more to the progress was actually detrimentally affected by my unwillingness and lack of initiative to communicate with my team. While I could equally blame others in the team, it wouldn't do any good to expect them to do something I knew would've made a difference: I was in a position to atleast help steer the team toward a more common goal or atleast have everyone be on the same page, but I completely failed to be proactive. Due to that, Alyssa, Adam, and some of the others had to pick up some of the slack while I just sort of made commits here and there, too afraid to try and commit anything else, as I was mostly doing the graph and didn't want to do more placeholder data, and wanted to start working with MongoDB Collections that I knew would be used and not be an obsolete method of data handling (as I was working with CSV parsing to load graph data before).

## Last takeaways and lessons
  Honestly, I really did feel that I failed my team due to my lack of communication and ability to efficiently contribute. While I did have the motivation and excitement to make progress in what I was tasked with, I feel that since we weren't well coordinated, and I was just too afraid to say anything, it made it harder for all of us to contribute as much as we could've been, despite us still getting a slightly functioning app running. I think I need to reassess how important communication is and not be afraid to try and just talk to my teammates, as the consequences can be pretty dire, as I've learned from this experience. I'm pretty thankful to have had the opportunity to work with these guys to make something more than just a homework or assignment; rather, something a little more "real" and impactful, which is something that I'm not really used to. With that, I'll leave the link to the GitHub repository and also the official site down below in case you're curious how it turned out. Thanks for reading my essay!

GitHub repository:[Kala Forecast repo](https://github.com/kala-forecast/kalaforecast)

Official site: [Kala forecast website](http://kalaforecast.org)


  
  
