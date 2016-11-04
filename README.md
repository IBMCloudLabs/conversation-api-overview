# Conversation API Overview

## Why, When, and How

Watson combines a number of cognitive techniques to help you build and train a bot - defining intents and entities and crafting dialog to simulate conversation. The system can then be further refined with supplementary technologies to make the system more human-like or to give it a higher chance of returning the right answer. Watson Conversation allows you to deploy a range of bots via many channels, from simple, narrowly focused Bots to much more sophisticated, full-blown virtual agents across mobile devices, messaging platforms like Slack, or even through a physical robot.

## Suggested uses

* Add a chatbot to your website that automatically responds to customers’ most frequently asked questions.
* Build Twitter, Slack, Facebook Messenger, and other messaging platform chatbots that interact instantly with channel users.
* Allow customers to control your mobile app using natural language virtual agents.

## Overview
With the IBM Watson™ Conversation service, you can create an application that understands natural-language input and uses machine learning to respond to customers in a way that simulates a conversation between humans. Your application can be an automated customer-service agent that is available from your website, a bot that communicates by using a chat service or social-media channel, a mobile app, or anything else that uses natural language to communicate with users. The Conversation service provides an easy-to-use graphical environment for creating natural conversation flows between your application and your users.

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
