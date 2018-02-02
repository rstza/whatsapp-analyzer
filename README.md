# Introduction

Whatsapp-Analyzer is a statistical analysis tool for Whatsapp chats. Using Matplotlib, it generates various plots showing, for example, the average number of words chat participants write per message. For the analysis it works on the chat files that can be exported from Whatsapp. Below you can see a selection of plots it produces when analyzing a group chat of mine:

![example](example.png)

# List of Plots

- Number of messages sent for each user
- Average words per message for each user
- Number of messages sent as share for each user
- Words written as share for each user
- Average number of messages in specific hour or weekday
- Number of messages mapped on days

# How to Use

To get started, you need to export the chat you want to analyze to your computer. To do that, open Whatsapp on your mobile phone and select the chat. Under **group / contact info** you will find the button **export chat** - choose **without media**.

Whatsapp is weirdly inconsistent with the format of exported files. Depending on OS and language, the time, date and status message format will be different. This program expects the following format:


```
dd.mm.yy, hh:mm:ss: Rose Marie: Darling! Its been an age! Tell me, how are you?
24.01.18, 09:03:56: Mary Jane: Simply splendid. I purchased a new estate: <image omitted>
```

Place your chat file named **_chat.txt** in the same directory as the analyzer. Alternatively you can hand over a file path as command line argument. Run `python3 analyzer.py [file path]` in your terminal to start the analysis. Switch between plots using the arrow keys.

# Needed Dependencies

- [matplotlib](https://matplotlib.org)
- [scipy](https://www.scipy.org)
- [numpy](http://www.numpy.org)

