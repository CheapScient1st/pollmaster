# Pollmaster

<br>Polling platform<br/>
<br>Author: Fengrui Gan, Felix Chung<br/>

Website for project 3 in [CS5610 Web Development](https://johnguerra.co/classes/webDevelopment_fall_2021/).

## Project Objective

<br>The objective is to build platform for people to create and to participate in polls<br/>
<br>This should be a React application.<br/>

## Proposal Goals

1. User registration/login.
2. All visitors can use a code to participate a poll
3. Poll maker can create polls with topic/questions and options/answers
4. Each poll will have an expiration time
5. Poll result should be updated automatically.

[Link to landing page](https://poll-master.herokuapp.com/)

![Home page of website](/images/main_page_ss/png)
![Demo of poll page](/images/poll_page_ss.png)
![Demo of create poll page](/images/create_poll_ss.png)
![Demo of poll list page](/images/poll_list_ss.png)




## Tech requirements

- The home page should be able to open on most browser
  -Chrome, Firefox, Safari, Internet Explore etc...

## How to Use?
- Registered users create a poll and share the generated link/code to other people.
- During poll creation, user can choose to have the poll to be puiblic or private.
    - public polls are available on the poll list page, private polls can only be access through links
- Users with link can copy and paste link to the browser to join a poll
- User with code can copy and paste the code to the search bar to join a poll

## Instruction to build

- When testing file, create your own .env file that inclode: DB_URL.
- Create a database and connect to your database in the backend
- Deploy these files on any server

## Database schema
### Poll Schema
- _id: (ObjectId)
- title: String
- options: Array(Object(prompt:String, votes: Int))
- owner: String
- totalVotes: Int
- public : Bool
- createdAt:Double
- ttl: Double
### User Schema
- _id: String
- firstName: String
- lastName: String
- password: String
- createdPolls: Array(ObjectID)
- votedPolls: Object(ObjectID: Int)

## Creator:
### Felix:
  - User login
  - User registration
  - User profile
  - Nav bar
### Simon:
  - Create poll page
  - poll page
  - poll list
  - home page
## [Video Demostration]()
## [Slides]()
