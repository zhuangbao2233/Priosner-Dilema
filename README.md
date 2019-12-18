# Priosner-Dilema
Project 1 In this project, you will develop bots that play a simple game. Each bot has a different strategy. You will pit these bots against each other to determine which strategy is more successful in this context. These bots are incredibly simple, and consist of a few lines of code and methods that represent different strategies of play.  Teams Teams have been assigned for this project and will be posted on Blackboard. They are fixed - no switching or cooperating across team lines. It is up to teammates to ensure that their partner adheres to the American University Honor Code. You may use pair programming, however, you must each take turns in the driver role on your own laptop. I should see commits on Github for each of you to get full credit for this assignment. 

Step 0 - Background Research. Both members should review the description for the Prisoner's Dilemma on Wikipedia. You do not need to become familiar with the intimate mathematical details of the Dilemma, just the general mechanism and the difference between the iterated dilemma and the non-iterated version (Introduction through the end of Section 3.1). This topic has been debated endless in a variety of fields, so there is a lot of additional material available if you want to dig deeper. For this assignment, you will only be required to be familiar with the basics (e.g., you will not need to understand the Nash equilibrium or the proof that goes with it). Both members should work together to devise five strategies for "winning" the prisoner's dilemma over a long number of iterations. I recommend first writing these strategies down in simple English rather than trying to jump directly into developing code. You may use the 'tit-for-tat' strategy as one of them, or come up with ones of your own. Optional There are several good videos that can help make these concepts a little clearer. I recommend this one, but there are many others.

Step 1 - Create the Repo for your Team. Both members of your team will visit this link. This will create a repo for your team in Github. For this assignment, you will share a Github repo with your teammate. If you are the first member of your team to visit the link, you can create the team and the repo - make sure you create the right team. If you are the second member to click the link, then make sure you join the right team. Both members will clone the repository to your local machines (i.e., using git clone &lt;URL>). You will then each have a local repository that is linked to the shared repository, and can work on the code together. As a reference for how to use git, I suggest this site, as it avoids some of the more complicated theory behind git and focuses on the bare minimum practicalities. 

Step 2 - Review the Provided Code. In the repository is a starter class, Prison, that has the bare minimum for the prisoner's dilemma. There is a variable for the last choice made by each of two prisoners, (i.e., Prisoner A and Prisoner B).  //The last choice of each prisoner.      boolean lastChoicePrisonerA = BETRAYED; //Set initially to BETRAYED for testing     boolean lastChoicePrisonerB; Two examples are given. Prisoner B is using a randomChoice() strategy, in which B will randomly choose to stay silent or betray Prisoner A. This strategy does not use prior information to make the decision - it is equivalent to flipping a coin. The provided code gives an example of a second strategy: betrayIfBetrayed(). If A betrayed last time, then B will betray also.

Step 3 - Write one method for each strategy. Following the design pattern for the example strategies, define one method for each of your team's five strategies (the example methods do not count). Assume that each prisoner can know the outcome of one or more previous encounters with the other prisoner through parameters passed to the method.

Step 3.5 - Commit and Push to Github Remember, this is not like using Blackboard for submitting assignments. As you are working with your teammate, you will need to frequently push code to the Github repo so that your teammate can access it. If you wait to the last minute, you could have conflicts that are difficult to resolve. It is much better to get into a rhythm with your partner early rather. To get full credit for your part in this, I need to see multiple commits from each team member.  

Step 4 - Write a method for scoring the outcome If they both stay silent then both prisoners serve 1 year. If a prisoner stays silent and the other betrays, then the prisoner who stayed silent gets 3 years in prison while the other goes free. If both betray, then each prisoner serves 2 years. Write a method that assigns a score to a strategy based upon the outcome. A high score is a bad thing, as each point represents a number of additional years added to the prisoner's sentence.
