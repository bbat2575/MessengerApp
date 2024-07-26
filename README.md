# Messenger App

**A role-based messenger app for academic purposes**

Messenger features:
- Friends list
- Chat rooms
- Message history
- Offline messaging
- Article repository
- Comment on articles
- Role-based commands
- Anonymity when posting articles and comments

*See passwords.txt for existing accounts and their sign in details.*

<img align="center" src="https://github.com/bbat2575/MessengerApp/blob/main/Messenger.png"> 

## Roles

Admin:  
- Can chat to anyone (Admin friends list contains every user that signs up).  
- Set/Delete roles for any user.  
- Mute/Unmute any user.  
- Create articles.  
- Modify/Delete articles created by any user.  
- Comment on articles.  
- Delete any comment.  

Staff (many different types of staff roles can exist):  
- Can chat with friends.  
- Mute/Unmute Student users.  
- Create articles.  
- Modify/Delete articles created by themselves or by Student users.  
- Comment on articles.  
- Delete comments made by themselves or by Student users.  

Student:  
- Can chat with friends.  
- Create articles.  
- Modify/Delete their own articles.  
- Comment on articles.  
- Delete their own comments.  

## Commands

Type "!" in chat box to see role-specific commands.

Admin Commands:  
- !role set <username> <role>  
- !role delete <username>  
- !mute <username>  
- !unmute <username>  

Staff Commands:  
- !mute <username>  
- !unmute <username>  

*Muted users cannot join chat rooms nor post or comment on articles.*

## Setup

To setup, install the packages:

```bash
pip install -r requirements.txt
```

## Running the App

To run the app:

```bash
python app.py
```

Navigate to `http://127.0.0.1:5000`

## A Warning
Since this app uses cookies, you can't open it in separate tabs to test multiple client communication. This is because cookies are shared across tabs. You'd have to use multiple browsers to test client communication.

## Tech Stack
- HTML
- CSS
- Javascript
- Python
- SQLite

## Javascript Dependencies
- Socket.io
- Axios (for sending post requests, but a bit easier than using fetch())
- JQuery (if you're familiar with web frameworks this is like the stone age all over again)
- Cookies (small browser library that makes working with cookies just a bit easier)

## Python Dependencies
- Template Engine: Jinja
- Database ORM: SQL Alchemy (use SQLite instead if you are an SQL master)
- Flask Socket.io
