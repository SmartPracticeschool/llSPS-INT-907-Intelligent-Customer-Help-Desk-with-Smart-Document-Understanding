# llSPS-INT-907-Intelligent-Customer-Help-Desk-with-Smart-Document-Understanding
Intelligent Customer Help Desk with Smart Document Understanding

## Project Description
A customer care chatbot can answer simple questions, such as store locations and hours, directions, and maybe even making appointments. In this project, the queries will be handled in a better way. If the customer's question is about the operation of a device,the application shall pass the question onto Watson Discovery Serviceand we can handle the queries in a better way. We will build a chatbot that uses various Watson AI Services like Watson Discovery, Watson Assistant, Watson Cloud functions and Node-Red and deliver an effective user friendly Web User Interface

The repository contains the Node-Red flow of the chatbot developed using various IBM Watson Services for backend and Node-Red for front end of the UI.

## How it Works
In Watson Discovery the data was enriched with the ecobee3_userguide.Then the annotation of document using Watson Dicovery SDU was done. It means that the Watson Discovery model will be trained so that the queries will be focused on the search for most relevant information from the document uploaded in Discovery. Watson Assistant will acts as the Chatbot with predefined standard dialogs to handle typical conversation between customer. When the query comes under technical domain, it will communicate with Discovery service with the help of 'Webhook'. Webhook was be created by defining a web action using Cloud Functions. Node-Red acts as a link between all the services utilized in this project and create a user friendly UI for the customers.

## Working Flow
The user interacts with Node-Red app UI. The chatbot engages the user in conversation.
Dialog in this interaction is coordinated by Watson Assistant.
If the customer asks a technical question, it will be passed to Cloud Functions action.
This action will further pass onto to Watson Discovery and return with appropriate solution.

Project demonstration video link: https://youtu.be/-_JDEFqL2kY

UI Link for project: https://node-red-jtsdv.eu-gb.mybluemix.net/ui/
