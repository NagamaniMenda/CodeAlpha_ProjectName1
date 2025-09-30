# CodeAlpha_ProjectName1


***ChatBot***

![ChatBot Screenshot](https://github.com/NagamaniMenda/CodeAlpha_ProjectName1/blob/main/chatbot.JPG?raw=true)

## Project Overview

Name: MENDA NAGAMANI
Company: CodeAlpha Internship Program
ID: CA/SE1/3702
Domain: Python Programming
Duration: September 1, 2025 – September 30, 2025

### Project: Python ChatBot

A beginner-friendly Python console project for an interactive chatbot.

## Description

The ChatBot interacts with the user by responding to greetings, moods, jokes, and simple questions. It is designed to be fun, interactive, and beginner-friendly.

## Features

* Responds to greetings
* Detects and responds to user moods
* Tells jokes and fun responses
* Answers basic questions like name and capabilities
* Exits on farewell commands

## How to Run in Jupyter Notebook

1. Open this repository in Jupyter Notebook or JupyterLab.
2. Open a new code cell.
3. Copy and paste the code below into the cell.
4. Run the cell to start the ChatBot.
5. Type your messages and see the bot’s responses.

## Example ChatBot Interaction

Welcome to the Extended ChatBot! (Type 'bye' to exit)
You: hello
Bot: Hello! How can I help you today?
You: tell me a joke
Bot: Why did the computer go to the doctor? Because it caught a virus! 😄
You: how are you?
Bot: I'm doing well, thanks for asking! How about you?
You: bye
Bot: Goodbye! Have a great day!

## Python Code

# Function to get chatbot response
def chatbot_response(user_input):
    user_input = user_input.lower()

    # Greetings
    if user_input in ["hello", "hi", "hey", "hola", "greetings"]:
        return "Hello! How can I help you today?"
    
    # Asking about bot
    elif user_input in ["how are you", "how are you?", "how's it going"]:
        return "I'm doing well, thanks for asking! How about you?"
    
    # User response to bot's mood
    elif user_input in ["i'm fine", "i am fine", "good", "great", "awesome"]:
        return "That's wonderful to hear!"
    elif user_input in ["not good", "bad", "sad", "tired"]:
        return "Oh, I'm sorry to hear that. Hope things get better soon!"

    # Fun responses
    elif user_input in ["tell me a joke", "joke", "make me laugh"]:
        return "Why did the computer go to the doctor? Because it caught a virus! 😄"
    
    # About bot
    elif user_input in ["what is your name", "who are you"]:
        return "I am ChatBot, your friendly assistant!"

    elif user_input in ["what can you do", "help", "assist me"]:
        return "I can chat with you, tell jokes, and answer simple questions!"
    
    # Farewell
    elif user_input in ["bye", "goodbye", "see you", "exit", "quit"]:
        return "Goodbye! Have a great day!"
    
    # Unknown input
    else:
        return "Sorry, I didn't understand that. Can you try saying it differently?"

# Main chat loop
def chat():
    print("Welcome to the Extended ChatBot! (Type 'bye' to exit)")
    
    while True:
        user_input = input("You: ")  # Get user input
        response = chatbot_response(user_input)
        print("Bot:", response)
        
        if user_input.lower() in ["bye", "goodbye", "exit", "quit"]:
            break

# Run chatbot
if __name__ == "__main__":
    chat()


## Project Info

Language: Python

Type: Console-based ChatBot

Level: Beginner-friendly
