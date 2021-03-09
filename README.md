# Mesh Video Conference

This is the Video Conference Web Application for making benchmark tests with mesh.

## Getting Started

### Installing

Nodemon is needed to run the Application.

```
npm i --save-dev nodemon
```

## Running the Application in localhost

To run the application in localhost, you need two consoles.

On the first console u start the Application:
```
npm run devStart
```

On the second console u start the peerjs port:
```
peerjs --port 3001
```

The application can be opend now on the web browser at localhost:3000

## Built With

Libarys we used in node:

```
npm i express ejs socket.io
npm i uuid
```
