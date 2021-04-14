# Interactive Physiotherapist Agent
**Purpose of our project:** Our conversational agent is created to hold a conversation of at least 30 turns. Each turn is an instance of a prompt and a bot response. The conversations are based on a user who needs exercises that aid in phsical therapy. The user lets the bot know of the specfic location of their injury as well as the type of pain they are experiencing. The bot then responds accordingly asking for more information to best determine what exercise would be best suitable.  

## Class Organization & How to compile and run the code.
Since we have integrated Google's DialogFlow API for our project, we have implemented a QueryHandler intent within our DialogFlow agent which collects the parameters from a user prompt such as the indicated pain, location of pain etc. Here we have our back-end. Based on the information gathered by the QueryHandler the back-end then calls the event that is attached to the correct intent. In other words, an intent is called by invoking an event from the back-end.

## Specifics about index.js:
WebCallIntent function - assigns a variable to an agent parameter; consider this funtion to be what gathers the parameters from the QueryHandler.  
CallEvent function - when this function is used to set a follow up event given a specific agent and event.  
If/Else statemets - identify location (body part that user inputs) in order to call the associated event.

[Breakdown of how a conversation is outlined](./outline.pdf)

# Updates for Assignment 3
## List of features implemented
- A simple GUI.  
- An extra topic. 
- 5 reasonable responses (when the user enters something outside the two topics). 
- Spelling mistakes (Fuzzy matching). 
- Entity Matching. 
- Synonym Recognition. 
- Sentiment Analysis. 
## Documentation
[How features are used to improve agent's conversation and snippets of a conversation to demonstrate the feature](./COSC310-%20Features%20Explanation.pdf)
  
[Level 0 Data Flow Diagram](./COSC310_Team15/blob/main/Level0_DFD.pdf)
  
[Level 1 Data Flow Diagram](./Level1_DFD.pdf)
  
[Summary of test cases](./COSC310-%20Test%20Cases.pdf)
  
[Sample output and limitations](./Sample%20output%20&%20limitations.pdf)
  
[Bonus:Design test cases using unit testing framework; test the correct intent metadata is extracted from the user query.](./testing/index-test.js)
  
[Final Documentation](./COSC%20310%20-%20Final%20Documentation.pdf)
  
# Updates for the Individual Project
**Details:** For this assignment I have taken the output of my teams A3 and continued development with it by adding on features. I have cloned my teams A3 repository and worked on my own repository from there.
## List of features implemented through use of public APIs
- Google Translate API - implemented as Google Cloud Translation API.  
- Google Places API. 

## Documentation
- Formal report submitted on Canvas: Includes a link to this ReadMe file as well as detailed explanations of APIs used.
- Presentation slides/Video presentaion submitted on Canvas: Includes a description of the program's conversation topic as well as to more details of how these features are used to improve conversation with the agent.
