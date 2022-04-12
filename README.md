# Simple Web Server

**Base**

```
npm init
```

***package.json***
```
{
  "name": "simpleserver",
  "version": "1.0.0",
  "description": "Very simple server",
  "main": "server.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "name author",
  "license": "ISC"
}

```
***Create first server from test***

```
const http = require('http');

const hostname = '127.0.0.1';
const port = 3000;

const server = http.createServer((req, res) => {
  res.statusCode = 200;
  res.setHeader('Content-Type', 'text/plain');
  res.end('Hello World');
});

server.listen(port, hostname, () => {
  console.log(`Server running at http://${hostname}:${port}/`);
});
```

```
node server.js
```

***Testing***
```
localhost:1337
```

***Starting Server***

```
npm start
```

```
node server.js
```
![image](https://user-images.githubusercontent.com/88910148/163048449-dd936f14-4004-4431-8ca0-ef91680034bd.png)



