# Synapse Scholar (AI Agent) *AI-Powered Help for Curious Minds*
*This is my submission for the kaggle capstone project*


![](https://github.com/TejasKathuria/Synapse-Scholar-AI_Agent/blob/main/synapse_flowchart.png)
### 1) Project Overview

The Synapse Scholar system is an interactive, multi-agent learning assistant built entirely using the Google AI Agent SDK (ADK).
It simulates a complete educational support ecosystem where different specialized agents work together to answer queries, explain concepts, summarize study material, generate quizzes, perform real-time research, and evaluate student responses.

It also includes:
•	A memory bank (stores last 10 interactions)
•	A logging system (tracks agent activity)
•	A central router that intelligently assigns tasks to the correct agent
 
### 2) Problem Statement

Students often face multiple learning challenges:
•	Difficulty understanding concepts
•	Need for simple explanations
•	Need to summarize long content quickly
•	Lack of good practice questions or quizzes
•	Difficulty finding reliable information online
•	Need feedback on answers
A single AI assistant usually cannot excel at all these tasks simultaneously.
 
### 3) Solution Statement

The project solves these problems by implementing a multi-agent AI architecture in which each agent specializes in a single capability.

The system:
•	Understands student queries
•	Routes them to the correct agent
•	Performs the required task (explain, summarize, research, quiz, evaluate)
•	Maintains short-term memory
•	Logs the entire process for transparency

This ensures accurate, fast, and context-aware educational assistance using only Google ADK.
 
### 4) Architecture

The system architecture is divided into the following layers:

1. Main Router
•	Acts as the control center
•	Takes user input
•	Stores memory and logs
•	Sends the query to the correct agent based on intent

2. Query Understanding Agent
•	Performs intent classification
•	Detects whether the task is:
o	explanation
o	summarization
o	quiz generation
o	research
o	evaluation
o	or regular chat

3. Specialized Agents

Each specialized agent handles one job only (Single Responsibility Principle).

4. Tools Layer
•	Google Search Tool (internet research API)

5. Memory + Logs System
•	Stores last 10 conversation entries
•	Tracks which agent was triggered, when, and why
 
### 5) Functions of Each Agent

a) Query Understanding Agent

Purpose: Intent detection
Functions:
•	Reads user query
•	Classifies it into categories
•	Helps the Main Agent route tasks correctly
 
b) Explainer Agent

Purpose: Concept explanation
Functions:
•	Breaks down complex topics
•	Explains in student-friendly language
•	Provides educational clarity
 
c) Summarizer Agent

Purpose: Efficient summarization
Functions:
•	Compresses long text
•	Produces short revision notes
•	Helps with quick learning
 
d) Quiz Generator Agent

Purpose: Practice question creation
Functions:
•	Creates 5-question quizzes
•	Uses difficulty level
•	Topic-based question generation
 
e) Research Agent

Purpose: Real-time information extraction
Functions:
•	Uses Google Search Tool
•	Fetches web data
•	Synthesizes results
•	Produces an AI-generated researched answer
 
f) Evaluator Agent

Purpose: Assess student answers
Functions:
•	Reads student’s submitted answer
•	Gives a basic score
•	Provides feedback
•	Helps improve understanding
 
### 6) Essential Tools and Utilities

1. Google AI Agent SDK

Core framework for agent creation, routing, and interoperability.

2. Google Search Tool

Provides real-time search capabilities for the Research Agent.

3. Memory Bank
•	Stores last 10 user/bot interactions
•	Maintains minimal short-term context

4. Logging System
•	Tracks each agent run
•	Stores timestamps
•	Helps debug or analyze system behavior

5. Sync + Call APIs
•	Used internally by all ADK agents
•	Handles message passing and tool execution
 
### 7) Conclusion

Synapse Scholar demonstrates a complete multi-agent educational system built purely using Google ADK, without relying on OpenAI APIs.

The modular architecture ensures:
•	Clean separation of tasks
•	High accuracy
•	Scalability
•	Real-time research capabilities
•	Transparent logging
•	Context-aware memory



### [Have a look at it's working on YouTube](https://youtu.be/BPAJ560gMVU)
