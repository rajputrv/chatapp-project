The backend server is started at port 5000 using express app.listen, the fontend is running as default by react at port 3000, we want to run them simultanously, so we run use concurrently module.

```javascript
    //in package.json of project folder
    "server": "nodemon backend/server.js",
    "client" : "npm start --prefix frontend"

    "dev": "concurrently \"npm run server\" \"npm run client\""

```
