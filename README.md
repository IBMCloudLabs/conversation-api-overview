# Conversation API Overview

## Why, When, and How

Watson combines a number of cognitive techniques to help you build and train a bot - defining intents and entities and crafting dialog to simulate conversation. The system can then be further refined with supplementary technologies to make the system more human-like or to give it a higher chance of returning the right answer. Watson Conversation allows you to deploy a range of bots via many channels, from simple, narrowly focused Bots to much more sophisticated, full-blown virtual agents across mobile devices, messaging platforms like Slack, or even through a physical robot.

https://www.ibm.com/watson/developercloud/conversation.html

## Suggested uses

* Add a chatbot to your website that automatically responds to customers’ most frequently asked questions.
* Build Twitter, Slack, Facebook Messenger, and other messaging platform chatbots that interact instantly with channel users.
* Allow customers to control your mobile app using natural language virtual agents.

## Overview
With the IBM Watson™ Conversation service, you can create an application that understands natural-language input and uses machine learning to respond to customers in a way that simulates a conversation between humans. Your application can be an automated customer-service agent that is available from your website, a bot that communicates by using a chat service or social-media channel, a mobile app, or anything else that uses natural language to communicate with users. The Conversation service provides an easy-to-use graphical environment for creating natural conversation flows between your application and your users.

## Workspace
Creating workspaces
The Conversation service natural-language processing happens inside a workspace, which is a container for all of the artifacts that define the conversation flow for a particular application.
Workspace overview
A single Conversation service instance can contain multiple workspaces. A workspace contains the following types of artifacts:

## Intents
An intent represent's the purpose of a user's input, such as a question about business locations or a bill payment. You define an intent for each type of user request you want your application to support. To train the workspace to recognize your intents, you supply lots of examples of user input and indicate which intents they map to. In the user interface, the name of an intent is always prefixed with the "#character."

## Entities
An entity represents a term or object that is relevant to your intents and that provides a specific context for an intent. For example, an entity might represent a city where the user wants to find a business location, or the amount of a bill payment. To train the workspace to recognize your entities, you list the possible values for each entity and synonyms that users might enter. In the user interface, the name of an entity is always prefixed with the @ character.

## Dialog
A dialog is a branching conversation flow that defines how your application responds when it recognizes the defined intents and entities. You use the dialog builder to create conversations with users, providing responses based on the intents and entities that you recognize in their input.
As you add information, the workspace automatically trains itself on the latest changes. You do not have to take any action to initiate the training.

## Architecture

![Architecture](./conversation_arch_overview.png)
* Users interact with your application through the user interface that you implement. Interfaces can include anything from a simple chat window or a mobile app to a robot with a voice interface or a chat bot communicating through a third-party service such as Slack, Twitter, or Facebook.
* The application sends the natural-language user input to an instance of the Conversation service in the IBM Cloud. The application connects to a workspace, which is a container for a particular dialog flow along with the training data that it uses. The conversation service interprets the user input in order to understand the user's intent. It then directs the flow of the conversation and gathers any information that it needs to satisfy that intent.
* The application can optionally use additional Watson services, such as Tone Analyzer or Speech to Text, to analyze user input.
* Based on the user's intent and the gathered information, the application interacts with your back-end systems to carry out the requested actions: answering questions, opening problem tickets, updating customer information, placing orders, or anything else that you want it to support.

Based on this architecture, the overall process of implementing an application that uses the Conversation service requires you to do following:
* **Configure a Conversation workspace**. The workspace contains the dialog flow for your application, along with the training data that is required to understand your customers' needs based on natural-language input.
* **Develop your application**. The application connects to the Conversation workspace and uses REST API calls to communicate with the service. It also integrates with any other systems that are required, including back-end systems and third-party services such as chat services or social media.

## Watch video
https://youtu.be/1rTl1WEbg5U

## Demo
https://conversation-demo.mybluemix.net/

## References
* (i)  Overview page: https://www.ibm.com/watson/developercloud/conversation.html
* (ii) Official Developer Documentation: https://www.ibm.com/watson/developercloud/conversation.html

## Lab 1
https://medium.com/ibm-watson-developer-cloud/create-your-slack-bot-with-conversation-api-node-red-a5bf82aad24d#.9tqexd8bu

## Lab 2
https://www.ibm.com/blogs/watson/2016/12/build-chat-bot/
