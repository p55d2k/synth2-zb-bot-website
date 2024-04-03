---
sidebar_position: 3
---

# How It Works

How does Synth Zaobao Bot v2 work?

## Logic for Answering Questions

There are 2 types of questions:
- 汉语拼音
- 词语填空

### 汉语拼音

For the 汉语拼音 questions, the bot uses the `pypinyin` library to convert the Chinese characters to pinyin. The bot compares the pinyin with the options provided and selects the correct answer.

### 词语填空

For the 词语填空 questions, the bot splits the question into 2 parts: the sentence and the blank. The bot then searches through the article/passage for the sentence and extracts the words around the blank. Lastly, it compares the words with the options provided and selects the correct answer.

## Selenium

Python's Selenium library is used to automate the process of answering the Zaobao questions. Selenium is a powerful tool that allows you to automate web browsers. It is commonly used for testing web applications, but it can also be used for web scraping and automating repetitive tasks.

Zaobao's website is loaded in a browser window using Selenium, and the bot interacts with the website by clicking on buttons, entering text, and submitting forms. The bot is able to answer the questions by analyzing the HTML structure of the website and finding the correct elements to interact with.

## User Interface

The bot uses the terminal as its user interface. When you run the bot, you will be prompted to enter your username and password for Zaobao. The bot will then log in to your account and start answering the questions. You can see the progress of the bot in the terminal, and it will display the questions and answers as it goes through the quiz.

## Logs and Answers

The bot saves the logs to the session in the `data/logs.txt` file. The logs contain information about the questions and answers that the bot encountered during the quiz.

The bot also saves the answers to the session in the `data/answers.txt` file. The answers file contains the questions and the bot's answers to them.
