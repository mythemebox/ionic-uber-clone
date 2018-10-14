# Firebase Setup

In this steps, we're going to setup our firebase project & obtain required firebase key

### create new firebase project

Navigate to https://firebase.google.com/ & login with your google account, then create new project

![create new project]( https://github.com/codesundar/ionic-uber-clone/blob/master/img/new-firebase-project.png "create new project")


### Enable Email Login

Navigate to Authentication, then enable Email login

![enable email login]( https://github.com/codesundar/ionic-uber-clone/blob/master/img/enable-email-login.png "enable email login")
    
### Updating Realtime Database Rules (NOT FIRESTORE)

Navigate to real-time database rules & update rules as follows.

    {
        "rules": {
        ".read": true,
        ".write": true
        }
    }
![update database rule]( https://github.com/codesundar/ionic-uber-clone/blob/master/img/update-database-rule.png "update database rules")

### Updating Storage Rules

Navigate to firebase cloud storage rules & update rules as follows

    service firebase.storage {
        match /b/{bucket}/o {
            match /{allPaths=**} {
            allow read, write: if request.auth != null;
            allow read, write: if request.auth == null;
            }
        }
    }

![update storage rule]( https://github.com/codesundar/ionic-uber-clone/blob/master/img/update-storage-rules.png "update storage rules")

**Note:** Here we haven't added any high security rule for testing purpose. later you can modify this as per your security concern.


## What you did ?

- created firebase project
- enabled email auth
- Updated firebase realtime database rule
- updated firebase storage rules
