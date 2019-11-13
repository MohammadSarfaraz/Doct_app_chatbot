# Doct_app_chatbot using Rasa X on Website

![rasa](https://d2z6c3c3r6k4bx.cloudfront.net/uploads/event/logo/1077848/2ed953fb073b5e91df6a2e4e10b20578.png)

## About Rasa

Rasa Stack is a set of open source machine learning tools for developers to create contextual AI assistants and chatbots. It is the leading open source machine learning toolkit that lets developers expand bots beyond answering simple questions with minimal training data. The bots are based on a machine learning model trained on example conversations. It consists of two frameworks:

## for more detail go to link below
[RASA X](https://rasa.com/docs/rasa/user-guide/installation/)


## details of this project

Online appointment using [RASA X](https://rasa.com/docs/rasa/user-guide/installation/) to take an appointment with the consultant doctor and take feedback from there meeting.I am using  rasa as a platform to create dialogue management and spacy for training the module.This project help the people to fixed an appointment online using chatbot which is easier and convenient for everyone who want to fixed an appointment with their consultant doctor. 

* It has two part-:
1. OnlineAppointment(where we fixed an appointment)
2. Feedback (take feedback from user or patients to take details of there meeting with there consultant doctor with their rating between 1 to 10)

* I used front end as html and css
* For backend i used rasa nlu and core


Here are some example given below--

![screenshot](https://github.com/MohammadSarfaraz/Doct_app_chatbot/blob/master/medi%20pict/Screenshot%20from%202019-11-13%2014-20-02.png)

![Markdown logo]()

* i used socket connectivity using web socket channel on credential file

# Websocket Channel
The SocketIO channel uses websockets and is real-time. You need to supply a credentials.yml with the following content:

socketio:
  user_message_evt: user_uttered
  bot_message_evt: bot_uttered
  session_persistence: true/false
The first two configuration values define the event names used by Rasa Core when sending or receiving messages over socket.io.

By default, the socketio channel uses the socket id as sender_id, which causes the session to restart at every page reload. session_persistence can be set to true to avoid that. In that case, the frontend is responsible for generating a session id and sending it to the Rasa Core server by emitting the event session_request with {session_id: [session_id]} immediately after the connect event.

The example Webchat implements this session creation mechanism (version >= 0.5.0).

REST Channels
The RestInput and CallbackInput channels can be used for custom integrations. They provide a URL where you can post messages and either receive response messages directly, or asynchronously via a webhook.

## for more detail 
 (go to this link)[https://rasa.com/docs/rasa/user-guide/connectors/your-own-website/]




