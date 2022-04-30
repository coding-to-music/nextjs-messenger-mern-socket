# nextjs-messenger-mern-socket

# 🚀 Javascript full-stack 🚀

### React / omdbapi.com API

This is a basic messenger web chat application. Where you can send private messages to online users. For this application is used sockets for sending messages, express for backend server with mongodb for saving data and on the frontend I used React with Next.js for search engine optimization.

https://github.com/coding-to-music/nextjs-messenger-mern-socket

https://nextjs-messenger-mern-socket.vercel.app

https://nextjs-messenger-mern-socket.herokuapp.com

by Domen Perko https://github.com/perkzen

https://github.com/perkzen/messenger

## Environment Values for .env

```java
MONGODB_URI="mongodb+srv://<userid>:<password>@cluster0.zadqe.mongodb.net/nextjs-messenger-mern-socket?retryWrites=true&w=majority"
```

![Screenshot](https://user-images.githubusercontent.com/73199603/152814175-12e08253-6e71-4ce1-aacb-daadaf576912.png)

This is a basic messenger web chat application. Where you can send private messages to online users. For this
application is used sockets for sending messages, express for backend server with mongodb for saving data and on the
frontend I used React with Next.js for search engine optimization.

## Getting Started

First you need to install all necessary packages on the frontend and backend:

```bash
cd frontend
npm i

cd backend
npm i
```

After that create a `.env` file in the backend folder, it should look something like this.

```dotenv
DATABASE_URL=mongodb+srv://<username>:<password>@cluster0.oop39.mongodb.net/<collection-name>?retryWrites=true&w=majority
PORT=5000

```

To start the application you need to run the frontend and backend server with the following commands.

```bash
cd frontend
npm dev

cd backbend
npm dev
```

If everything works correctly you should get these two outputs in your terminal windows.

For frontend:

```bash
ready - started server on 0.0.0.0:3000, url: http://localhost:3000
event - compiled client and server successfully in 553 ms (307 modules)
```

For backend:

```bash
Server is running on port 5000
MongoDB database connection established successfully
```

## Project details

NodeJS version: 14.18.1

Express version: 4.17.2

ReactJS version: 17.0.2

Typescript version: 4.5.5

Next version: 12.0.8

### Important frontend packages

- next
- redux
- redux-saga
- redux-toolkit
- typescript
- react-hook-form
- classnames
- uuid
- sass
- react-icons
- axios
- socket.io-client
- emoji-picker-react
- @dicebear/avatars-identicon-sprites
- react-intersection-observer

### Important backend packages

- bcrypt
- cors
- express
- mongoose
- socket.io

## GitHub

```java
git init
git add .
git remote remove origin
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:coding-to-music/nextjs-messenger-mern-socket.git
git push -u origin main
```

## Heroku

```java
heroku create nextjs-messenger-mern-socket
```

## Heroku MongoDB Environment Variables

```java
heroku config:set

heroku config:set MONGODB_URI="your value"
```

## Push to Heroku

```java
git push heroku

# or

npm run deploy
```
