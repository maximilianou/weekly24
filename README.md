# TODO: A Chat System, webwockets, docker, Redis publish/subscribe, MongoDB

```
For our engineering test, we'll be looking at a few things. The experience overall with designing a simple application and communication ability in explaining how/why you chose what you did. 

Timeline: One Week
Requirements:

Use Docker and docker-compose.

Use modern LTS Node.js version.

Don’t use common ports for the app running (80, 8080, 3000, etc.). The app shouldn’t conflict with other processes on our dev machines.

Use native WebSockets API for browsers.

Don’t use the Socket.IO library.

Use worker_threads module.

Use Redis pub/sub mechanism.

You need to create a simple Chat Room where any user can join by basic URL (“/”), no authentication needed. After the page loads, a user should enter his name. After that, he should be connected to the Room. The room contains an input where a user can enter his message and a button for sending it. Messages sending should be implemented with WebSockets. New messages should appear in the chat section of the page.

The application should use the “worker_threads” module and utilize all available CPU cores. It could run on a single port or different ports.

A chat message that was sent from frontend to backend, should be published to other app threads by Redis publish/subscribe mechanism. In this way, every connected user to the room should receive the chat messages independently of port/thread to where he’s connected. We should emulate multi-threads/servers communication in this way.

Each chat message should be saved to MongoDB. So, each newly connected user can see all previous messages. You can use an API endpoint or WS event for fetching messages from the backend (it’s your choice).

The frontend of the app should be a simple HTML page with included JS, CSS files.


Review of the project:

Create a small schema of your architecture

Open Loom or a Screen recording tool

Record a video and walk through your architecture of the task explaining it in simple terms (imagine you are explaining this to the product team)

Open the application and explain why you chose an API endpoint or a WS in your test project. What was your logic here?

Please explain how you could scale this further to support a thousand messages at one time (what are scale concerns for us to worry about?)

Submit video with the test application

Thank you so much for your time so far and excited to learn more!

```

