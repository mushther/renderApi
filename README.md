# mock-api\_

# step 1: Create a repository

# step 2: clone it locally

# step 3: add package.json to the file ,Just do npm init in terminal

# step 4: Install json-server with command npm install json-server cors json-server

# step 5: add a file with name index.js

# step 6: add to the dependencies in script "start": "node index.js"

# step 7: add below line of code in index.js

const jsonServer = require("json-server");
const server = jsonServer.create();
const router = jsonServer.router("db.json");
const middlewares = jsonServer.defaults();
const port = process.env.PORT || 8080;

server.use(middlewares);
server.use(router);

server.listen(port);

# step 9: add a file with name db.json and put all your data in db.json file

{
"products":[
{id: 1, name: "html"},
{id: 2, name: "css"}
]
}

# step 8:push these code with command

1-git add .
2-commit -m "msg"
3-git push

# after this go to the `render.com` open your accout with github

# after successful login you will get "New+" button left side of username, Click on then get webservice

# after clicking on webservice you will get connect button with your repositories name , click on connect

# after you will get input to type service name ,here u can type service name any ?

# after this scroll down to bottom ,u will get button `create webservice` just click on it ,it will deploy and provide a link on top left side.
