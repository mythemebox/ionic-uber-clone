# Admin Panel Setup

## Creating Admin Account

To login with your admin panel, first you need to create an email account from your firebase.

![creating admin account]( https://github.com/codesundar/ionic-uber-clone/blob/master/img/create-admin-email.png "update database create admin account")


## Updating Configuration

- Navigate to `driver/src/environments/environment.prod.ts`
- Update firebase credentials
- navigate to `admin/src/app/login/login.page.ts` & update newly created admin email


## Running Admin Panel

once you have done, now you can serve into browser.

    cd admin
    npm install
    ionic serve

## Set Default cars & price value

Navigate to Cars / settings page & press **SET DEFAULT** button.


### What you did?

- Created admin email manually from firebase
- Updated admin email on login.page.ts
- Running admin panel
- Set default vaules (For cars)
