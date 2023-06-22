# Software design 

# Requirements and features 

Since COVID-19, it has become normal to work from home for a few days a week. However, this does make it more difficult for colleagues to find each other and ask question. IO wanted a solution to this. They wanted a mobile app that shows where each employee is working. 
If this is from home or at the office and where in the office, they are.  

 

As a user, I want to ping a co-worker with the message that I am looking for them, so my colleague knows I want to speak to them. 

As a user, I want to receive a notification when a specific co-worker is not in a meeting anymore, so I can send them a message that I want to speak to them. 

As a user, I want to be able to favourite a co-worker because this makes it easier to find the colleagues I work with the most. 

As a user, I want to be able to look for a specific colleague in a search bar because this makes finding people on the app easier.  

As a user, I want my location to be updated automatically based on what wifi point I am connected to. 

As a user, I want to be able to update my own location.  

 
 

# User Interface 

To give an idea of what the user interface would look like, designs were made.  

The first decision that had to be made were the colours. We requested IO to send us their colour schemes and they did. Based on this we started creating designs. 

![image](https://github.com/SoleilUmwiza92/PortfolioS3/assets/124836754/165dde6e-50f6-4ccb-8c19-db5bb1476d19)


Figure 1. IO colour scheme 




The second step was making the actual designs. We started with a dashboard with log in screen.  

![image](https://github.com/SoleilUmwiza92/PortfolioS3/assets/124836754/a88d2221-48c4-4a1d-bdf5-b9a62007e262)


Figure 2. Log in screen, dashboard and menu 




![image](https://github.com/SoleilUmwiza92/PortfolioS3/assets/124836754/32f01984-ac6f-4ec0-923b-c86888147ad1)


Figure 3. Search page, search bar filled in and individual information 





![image](https://github.com/SoleilUmwiza92/PortfolioS3/assets/124836754/768891c4-a395-42c8-8ec0-7c83d559400b)



As there are also notifications to respond to, an interface had to be made for this. This can be seen below. 




 ![image](https://github.com/SoleilUmwiza92/PortfolioS3/assets/124836754/b397306b-387e-4ed2-a7c5-497ab0b439d7)
 
 Figure 4. Individual information and a ping notification 

 

# Software Architecture  

Secondly, a software architecture was made. The different layers of the application are highlighted here, those being: Presentation, Business and Data.  

 

The presentation layer includes the User Interface, which is what the user sees and what the designs were shown from in last chapter. Then the Presentation Logic, this includes all the processes that go on behind the scenes that the user does not see but that do still happen in the frontend. An example of this is the ping notifications. These are mostly managed from the frontend; this is something that will be discussed later on.  

The second layer is the Business layer. This layer contains the API and the data handling. It is responsible for getting the data from the database and sending it to the frontend but also sending the data given in the frontend to the database. Two parts of this are the Employee Controller and the Employee service. 
These two make sure that the data gets to the database in the correct format and are useable. Another part of is the Notification Service. 
This is responsible for sending a signal to the frontend when someone is out of a meeting. The frontend is then responsible for sending the notification.  

The last layer is the database. This layer is purely responsible for saving the data and sending it when the API requests it.  

![image](https://github.com/SoleilUmwiza92/PortfolioS3/assets/124836754/5916d299-0be9-4a42-a298-9bd1eff7c43f)

 

 
 

# API Endpoints 

One of the vital parts of the application is the API that makes sure the information is send to the database in the correct format and without missing information. The API has access points which are only meant to be accessed by authorized users. These access points are made in a CRU structure.  

The decision was made to use this structure since deleting or archiving the user was not the priority.  

# Accessing the API  

As it is an API, there are endpoints. In this case the endpoints would be: 

![image](https://github.com/SoleilUmwiza92/PortfolioS3/assets/124836754/88c3d54a-06c8-4194-bfaf-6689bbbf07b8)





 
