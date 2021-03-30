# ChatApp

Unit 8: Group Milestone
===
# TUNIN

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
2. [Schema](#Schema)

## Overview
### Description
It allows people to create two types of chat rooms teams and group. Teams chat consists of up to four people to communicate in a neat and concise way while group chat will be the standard chat which consists of more than four people. Its purpose is to remove confusion and avoid the convoluted paragraphs of other chat apps. 

### App Evaluation
- **Category:** Social Networking 

- **Mobile:** This app is an extension of a computer version that was previously created by one of the members. 

- **Story:** Made specifically for professionals who typically work in a team to help them communicate better.

- **Market:** This app can be used by anyone. 

- **Habit:** This app could be used as often or sporadically depending on how much users have to communicate with other users.

- **Scope:** The creator of the Group chat or Team chat would decide who would be placed into the created sub-chat rooms.

## Product Spec
### 1. User Stories (Required and Optional)

**Required Must-have Stories**

* Create chat room 
-Team chat (Max 4 people)
-Group chat (No Limit) // can have sub chat rooms (multiple team chats)
* Join chat room 
* Private message (quick message)
* Optional login // does not save the conversations 
* Login // saves the conversations 

**Optional Nice-to-have Stories**

* Add pictures / pdf
* Add movies / videos
* Add gifs / links
* Add audio files
* Message timestamp
* Play back messages
* Implement contacts
* Secondary chat name // way of naming a chat that only the person who wrote it can see
* Import conversations from other apps
* Invite system
* Contact request // friend request
* Settings (Accesibility, Notification, General, etc.)

### 2. Screen Archetypes

* Create / Join A Chat Room Screen (No need for logging in)
* Create / Join A Chat Room Screen (Logged in Version)
* Group Chat (Messaging) Screen
* Team Chat (Messaging) Screen
* Private Chat (Messaging) Screen

### 3. Navigation

**Flow Navigation** (Screen to Screen)
* Create A Chat -> Team/Group Chat Screen
* Join A Chat -> Team/Group Chat Screen

## Wireframes

![](https://i.imgur.com/xbHn78F.png)

## Schema
### Models

**Chat**


| Property | Type | Description |
| -------- | -------- | -------- |
| objectId     | String     | Id for users|
|created |DataTime |Chat created|
| updated | DataTime |Chat updated|
|Image |File|Image posted |
|messageCreated |DataTime|Message created|
|messageEdited|DataTime|Message edited|
|messageDeleted|DataTime|MessageDeleted|
|Video|File |Video posted|

### Networking

**List of network requests by screen**
* Home Feed Screen
    * Create - creates a new chat room
    * Join  - joins an existing chat room
* Chat Screen
    * Private chat - message individuals without creating a chat room
    * Delete chat- deletes chat rooms no longer used (@ user discretion)
    * Delete message - deletes messages
    * Edit message - edit messages
