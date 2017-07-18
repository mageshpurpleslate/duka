# Duka - Corporate Procurement Assistant

## Motivation behind it

Employees in corporate, would need to purchase things for their daily need. While corporate has a list of items to offer for employees, letting employees choose the items they want would help in multiple ways.

- Avoids discrepancy from what is needed and what is purchased
- Employee satisfaction
- Employee may get to see what best alternatives available 
- Creates a transparent purchasing process
- Can help to automate purchasing process

## What does _ Duka _ do? 

Duka means shop or store in Swahili. 

** Usage Instructions **
- Duka Bot can be installed by corporates slack admin. 
- Admin can create a slack channel for procurement and invite procurement team there. 
- Admin can invite employees to Duka Bot
- Employees can go to Duka Bot and look for items
- Duka will identify the intent and provides more filter for employees to narrow down items (defined as slots)
- Based on employee choices, Duka calls Amazon AWS API to search for the items
- Top 4 items listed for employee to choose
- Once employee chooses, Duka posts the request to procurement team 

## How we built it

- Used Amazon lex to create intents and slots
- Built lambda functions for the intents fulfilment
- lambda functions developed in Node.JS
- Used AWS LIB to query Amazon stories to get the products
- Used Slack API to post "employee request" 

## Challenges we ran into

- More examples on AWS Lex could have been better. For example, we took long time to find out, you need to choose _ latest _ in version in order to edit the lex definition
- Moving from one intent to another intent was a challenge. 

## Accomplishments that we're proud of

- Learning and Developing in the shorter time
- Integration with Amazon API

## What we learned

- AWS Lambda how it can change the future of server-less architecture
- AWS Lex and Bot Building

## What's next for duka

- Provision for companies to create their own shopping list

- Once employee selects  an item, further options to be derived automatically
   Example, once employee selects “Buy Laptop”, laptop brand and models to be taken directly from Amazon, 
   instead of current slots

- Approval workflow within Slack and the same status can be shown to employee

- Order placement can be done upon approval, but needs to be integrated with  Amazon API for shopping

- Order tracking information can be given to employee

- Voice Integration
