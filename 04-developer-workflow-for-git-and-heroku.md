<link href="index.css" rel="stylesheet" type="text/css">

# <a id="top">Chapter 4: Developer Workflow for Git and Heroku</a>

  Once you have created your application and deployed it on Heroku for the first time, you have a very simple deployment workflow for your projects.  Each time you make a meaningfull change to your project it is commited to your local  git repository.  When you have a one or more commits that you want to deploy, then you push them to the heroku git repository and the new version of your application is deployed.
  
  You get into the following cycle:
  
    # add / change your source code
    git add file(s)
    git commit -m "message"
    git push heroku master 


## Modify your project

  To demonstrate this workflow around Git and Heroku, lets make some simple changes to the new application. 
  
  First lets change the code to order the names on the leaderboard in alphabetical order.  Edit the file leaderboard.js and change the sort order in the Template.leaderboard... function:
  
    [TODO: insert code here and link to a file/git/git repository with the code changes] 
  
  *Rather than type in the code, you can also checkout the ... branch of the code in the github repository with the command git checkout list-assending* 
  
[TODO: create a project with branches for the different sections of the workshop, using symantically meaningful names.]

  Assuming you still have your the Meteor server running locally, it will detect the changes in your code and update your application immediately.  This gives you fast feedback on how your code behaves when its deployed.
  
  If all is well with you application, then we can deploy it to Heroku.


## Push your changes to Heroku

  Use the developer workflow to push this change to Heroku and update your live application:
  
    git add .
    git commit -m "leaderboard listed in asscending alphabetically order"
    git push heroku master 

  Now you have an updated live application.
  
## Modify your project again 

  Next, we add a button to the application to toggle the order of the leaderboard.



## Push your changs to Heroku again 

  Again, use the developer workflow to push this change to Heroku and update your live application:
  
    git add ...
    git commit -m "leaderboard listed in asscending alphabetically order"
    git push heroku master 



[TODO: check if meteor refreshs the browser connected to it when you deploy another release on Heroku.  As it effectively is a new "instance", does it know about the cients connected to it].

[Back to top...](#top)
[Chapter 05 - Tracking deployments]()
[Back to Workshop home](index.html)

