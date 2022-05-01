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
MONGODB_URI="mongodb+srv://<userid>:<password>@cluster0.zadqe.mongodb.net/nextjs-messenger-mern-socket?retryWrites=true&w=majority"
PORT=5000

```

To start the application you need to run the frontend and backend server with the following commands.

```bash
cd frontend
npm run dev

cd backbend
npm dev dev
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

## Debugging - Troubleshooting connection issues

https://socket.io/docs/v4/troubleshooting-connection-issues/

Please make sure the Socket.IO server is actually reachable at the given URL. You can test it with:

```java
curl "http://localhost:5000/socket.io/?EIO=4&transport=polling"

```

which should return something like this:

```java
# mine
0{"sid":"EgEdOYSW92CZrvUUAAAO","upgrades":["websocket"],"pingInterval":25000,"pingTimeout":20000,"maxPayload":1000000}

# example
0{"sid":"Lbo5JLzTotvW3g2LAAAA","upgrades":["websocket"],"pingInterval":25000,"pingTimeout":20000}
```

If that's not the case, please check that the Socket.IO server is running, and that there is nothing in between that prevents the connection.

## Can't push to Heroku, get build error:

```java
emote:        > frontend@ build /tmp/build_f02ea0dd/frontend
remote:        > next build
remote:
remote:        warn  - No build cache found. Please configure build caching for faster rebuilds. Read more: https://nextjs.org/docs/messages/no-cache
remote:        Attention: Next.js now collects completely anonymous telemetry regarding usage.
remote:        This information is used to shape Next.js' roadmap and prioritize features.
remote:        You can learn more, including how to opt-out if you'd not like to participate in this anonymous program, by visiting the following URL:
remote:        https://nextjs.org/telemetry
remote:
remote:        info  - Checking validity of types...
remote: Failed to compile.
remote:
remote: ./components/ChatInput/ChatInput.tsx:52:14
remote: Type error: 'Picker' cannot be used as a JSX component.
remote:   Its element type 'ReactElement<any, any> | Component<IEmojiPickerProps, any, any>' is not a valid JSX element.
remote:     Type 'Component<IEmojiPickerProps, any, any>' is not assignable to type 'Element | ElementClass'.
remote:       Type 'Component<IEmojiPickerProps, any, any>' is not assignable to type 'ElementClass'.
remote:         The types returned by 'render()' are incompatible between these types.
remote:           Type 'React.ReactNode' is not assignable to type 'import("/tmp/build_f02ea0dd/node_modules/@types/react/index").ReactNode'.
remote:
remote:   50 |         {visible && (
remote:   51 |           <div className={classes.Picker} ref={pickerRef}>
remote: > 52 |             <Picker onEmojiClick={onEmojiClick} />
remote:      |              ^
remote:   53 |           </div>
remote:   54 |         )}
remote:   55 |       </form>
```
