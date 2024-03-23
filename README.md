# ResumeAI

## Overview

Deploying ResumeAI Application :

BACKEND :
1. git clone the repo.
2. "npm i --force" - install node modules for the backend folder. 
3. create .env file with the required variables.
4. Generate secret keys for JWT and OpenAI.
  - for openAI = Login into your openAI account and generate secret key.
  - for JWT = random and unguessable string - better use "console.log(require("crypto").randomBytes(32).toString("hex"));" this code and save it a new file "generatekey.js" and run the file "node generatekey.js", resulting in a hexadecimal random string.
5. "tsc --project tsconfig.json" - Compile the typescript code, If typescript installed globally.
6. "nohup node src/main/index.js &"  (or)  "nohup npm start &" - to run the backend server.
7. If the above command to run the server throws an error, use "npm start" for backend application.

FRONTEND :
1. "npm i --force" - install node modules.
2. "npm install -g @angular/cli" - install angular.
3. "npm start" - to run the frontend server.
