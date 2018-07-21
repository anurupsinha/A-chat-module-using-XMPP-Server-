# A-chat-module-using-XMPP-Server-
During summer 2018, I did a 1 month internship at Tivintis Media Junction Pvt. Ltd., Kolkata. This was the project I was asked to prepare. Theey needed a sample chat module which allows group chat as well as one-to-one chat beside a video player like twitch. They wanted to use it on their video streaming sites. This uploaded project contains stuff by me as well as others which I used in my project.

# Setting up the Openfire server:-
1. Setting up the server is quite simple since it's completely GUI based.
2. During the initial configuration, there is an option of embedded databse or external database.
   Since, we want more number of simultenous connections, we have to choose External DB.
   The list of supported External DBs are displayed.
3. Once set up, there are various plugins available to download. 
4. The Candy Plugin is a must for the group chat module to work, so, do download it.
5. After setting up the server, the id for logging in into admin console is "admin" and 
   password is whatever you have set.
6. Users and chat rooms have to be created from the Openfire admin console initially.


# Changes in the Webpages:-
1. The page layout and styling have been done with simple HTML, CSS and JQuery codes.
2. Modification can be done wherever required.


# Connection:-
1. Connections are made by calling functions from the "strophe.js" library and wherever it is called,
   the IP address has to be updated to the IPV4 address of the Openfire hosting  machine.
2. The port will always be 7070. Openfire runs on port 9090 so do keep it available.
3. The domain after username also must be modified.


# Login.html:
1. While loggin in, just provide the username like jtv123. No need to provide the "@something.com" part.
2. Once logged in, the entered user-id and password is stored in the browser local storage and is used to login
   into the chat module.
3. After login the user is taken to the Video.html page


# Video.html:
1. This is the main page of our project.
2. In this page, the video is played using the default HTML video player and beside that is our chat module.
3. The chat module is basically a frame implemented using <iframe> tag of HTML.
4. By default, it enters group chat.
5. There are two hyperlinks right below to switch between Singe Chat (one to one) and Group Chat.
6. The frame changes accordingly.
7. Below that, is a list of videos that can be played. Clicking on one of them plays the video.
   As of now, we only have two videos.
8.In the right most corner at the bottom of the page, is the LOGOUT button.
  Clicking it, takes us back to the "Login.html" page and the user is asked to enter his credentials again.


# JavaScript Libraries Used:-
1. "strophe.js", "jquery-ui.js", "jquery.js".
2. "chat.js", used for single chat, is customised by us in accordance with our needs.
3. The Candy Project from Github (open Source), is a set of libraries which has used to develop our group chat module.
   There is no major change apart from minor styling and configuartion changes to run on our machine and server.
   The advantage of using Candy is it can be easily extended with the help of plugins which can be developed by us.
   A large number of open source plugins are available at the Github Candy plugins page.

 
 # ** No illegal use of license has been done and the original sources have been adequately mentioned in the 
 #    References part of my Project Report. **

