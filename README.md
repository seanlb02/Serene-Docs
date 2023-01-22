# SERENE - Documentation 

## Site Description

### Purpose 

 
Nowadays, around 20% of adults are suffering from mental illness. It affects a person a lot which shows on a person’s act.  This app is a platform which helps a user to track his mental health condition. There are some other purposes of this app which are given below-
 
Serene is a mental health journaling platform that gives users – and other users they authorise – the ability to log and track changes in their emotional state through time.
·  	Serene was built to solve the problem people face in recounting discrete changes in their mental health and disclosing these changes to those closest to them.
·  	Most of the time, people don’t want to disclose their mental state to others. But for special purposes such as monitoring (e.g. data can be monitored by the psychologists), users can grant access to other users.
·  	This app will help to understand a user’s mood so that he/she can manage them and feel better faster. Also, it’s easier to make decisions related to health which can provide a better quality of life.
·  	It is beneficial for a person to manage low moods and triggering situations if he/she tracks his/her mood daily through this app.
·  	Serene does this by allowing users to log their mental state each day via journal entries and a weekly wellbeing questionnaire, with select data summarised by a weekly/daily graphical snapshot. Users can grant other users access to this snapshot for remote monitoring. 
·  	This app plays a great role to reduce the stigma as in most of the communities, mental illness isn’t widely talked about.



### Functionality/features 

- A homepage includes a hero component and a Sign-in/Sign-up button for direct user auth access
- Ability for users to add short journal entries with accompanying ‘emotion’ tags
- A simple mental wellbeing questionnaire – optionally answered weekly 
- Ability for users to view a daily, weekly and monthly summary of their mental wellbeing, as recorded with journal entry tags and questionnaire results. 
- Ability for users to grant access to their weekly summary to select users

### Target Audience 

Although all demographics are welcomed to user Serene, it is initially targeted at therapists/social workers by providing a way to remotely track the mental health of the people under their duty of care.
  
## Tech Stack 

### <u>Front end</u>

React, Bootstrap

### <u>Back end</u>

Express/Node js, MongoDb, Mongoose 

### <u>Testing</u>

Vitest, Jest

### <u>Deployment</u>

Railway 

## Data Flow Diagram

![](./assets/dataflow.jpeg)

## Application Architecture Diagram



![](./assets/architecture.png)

## User stories 

Home 
- User must be able to register and sign in to their profile 
- User should be given a summary of what the app does 

Profile 
- User should have constant access to navigation via a navbar
- User should be able to see their username, welcome message and inspirational quote

Journal [profile component child]
- User should be able to post a journal entry with text, an ‘emotion’ tag and timestamp at any time
- User should be able to see a list of previous journal entries
- User should be able to delete posts


Weekly summary [profile component child]
- User should be able to see a summary of the past 30 days, that for each day shows (1) date (2) questionnaire score/colour (3) tags posted 

Questionnaire [profile component child]
- Each week a user should have the opportunity to answer a mental wellbeing questionnaire that gives them a score out of 10-50  
- User should have this score stored with a timestamp in the db
- User should be blocked for completing the questionnaire more than one time per week

Grant Access [profile component child]
- User should be able to see a list of usernames that have given them access to view their calendar (trackers) 
- Users should be able to search and add usernames to a list of people who can view THEIR summary (populate ‘tracking’ field in db collection)

Settings 
- User must be able to delete their account


## Wireframes 

High-resolution wireframes located in /assets/Wireframes.

### <u>Sign up</u>

![](/./assets/wireframe%20screen%20comparison/loginwire.png)


### <u>Log in</u>
![](/./assets/wireframe%20screen%20comparison/signupwire.png)

### <u>Profile</u>
![](/./assets/wireframe%20screen%20comparison/homewire.png)

### <u>Journal</u>
![](/./assets/wireframe%20screen%20comparison/journalwire.png)

### <u>Questionnaire</u>
![](/./assets/wireframe%20screen%20comparison/questionairewire.png)

### <u>Summary</u>
![](/./assets/wireframe%20screen%20comparison/summarywire.png) ![](/./assets/wireframe%20screen%20comparison/summarymobile.png)



### <u>Settings</u>
![](/./assets/wireframe%20screen%20comparison/settingswire.png)

## Trello Screenshots 
(https://trello.com/b/MMurIsLO/mern-frontend-kanban)  

![](/./assets/trello2.png)
![](/./assets/trello3.png)
![](/./assets/trello1.png)