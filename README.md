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
## Built With

Libarys we used in node (already included in node_modules, so dont need to install extra).

```
npm i express ejs socket.io
npm i uuid
```
