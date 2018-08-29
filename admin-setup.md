# Admin Panel Setup

## Creating Admin Account

To login with your admin panel, first you need to create an email account from your firebase.

![creating admin account]( https://github.com/codesundar/ionic-uber-clone/blob/master/img/create-admin-email.png "update database create admin account")


## Updating Configuration

- Before running app, open your `admin/src/app/app.component.ts` then update your firebase configuration.
- navigate to `admin/src/pages/login/login.ts` & update newly created admin email


## Running Admin Panel

once you have done, now you can serve into browser.

    cd admin
    npm install
    ionic serve

## Set Default cars & price value

Navigate to Cars / settings page & press **SET DEFAULT** button.