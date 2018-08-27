# Firebase Cloud Function Setup

Before doing firebase setup, we need to install firebase tools on your machine. To do that, please execute
    
    npm install -g firebase-tools

**Create new project & login to firebase** 

    mkdir fcf
    cd fcf
    firebase login
    firebase init functions

It might asks your few questions, please answer as followed

- Choose your firebase project
- Language: JavaScript
- EsLint: No
- Npm install: Yes

Once it's created functions/index.js & functions/package.json then follow these steps

    cd functions
    npm install --save firebase-admin
    npm install --save firebase-functions
    npm install --save stripe

Then replace your newly created index.js with downloaded index.js & also update your stripe api key inside index.js

    cd ..
    firebase deploy --only functions

**Note:** You must be inside fcf/ (not inside fcf/functions) folder for deploying.