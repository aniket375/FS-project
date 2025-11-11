# Call-Me

This project enables easy one-to-one video calls directly from your web browser using WebRTC technology.

![callme](./assets/doc/callme.png)

## Getting Started

### Overview

This project allows you to:

- `Sign in` with a username.
- `Initiate video calls` by clicking the call button next to a recipient's username.
- `Switch` between cameras, microphones, or speakers seamlessly during a call.
- `Chat` in real time with all participants.
- `Hide` your video feed as needed.
- `Toggle` your audio.
- `Toggle` your video.
- `Toggle` your screen.
- `Hang up` the call when finished.
- `Use the REST API` to retrieve the list of connected users or initiate a call.

---

### Quick Start

- #### Using NodeJs

![nodejs](public/assets/nodejs.png)

**[Install Node.js and npm](https://nodejs.org/en/download)**

```shell
# Clone this repo
git clone https://github.com/miroslavpejic85/call-me.git

# Go to to dir call-me
cd call-me

# Copy the config file
$ cp public/config.template.js public/config.js

# Copy .env.template to .env
cp .env.template .env

# Install dependencies
npm install

# Start the application
npm start
```

---



1. `Open` your browser and visit [http://localhost:8000](http://localhost:8000).

2. `Sign in` with your username.

3. `Select` the connected recipient's username and click `Call`.

4. `Enjoy` your one-to-one video call.

---

## Click to Call

Allows a user to `join` the room as a `user1`

- [http://localhost:8000/join?user=user1](http://localhost:8000/join?user=user1) (dev)
- [https://cme.mirotalk.com/join?user=user1](https://cme.mirotalk.com/join?user=user1) (prod)

Lets the `user2 join` the room and initiate a `call` to the `user1`

- [http://localhost:8000/join?user=user2&call=user1](http://localhost:8000/join?user=user2&call=user1) (dev)
- [https://cme.mirotalk.com/join?user=user2&call=user1](https://cme.mirotalk.com/join?user=user2&call=user1) (prod)

You can explore a `widget` example that demonstrates this functionality [here](./integration/widget.html).

---

