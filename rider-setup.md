# Rider App Setup

### Update Firebase Rules

- Navigate to `rider/src/app/app.module.ts`
- update your firebase configurations
- Update your Google maps api & stripe public key with `rider/src/index.html`

### Running Rider App

    cd rider
    npm install
    ionic serve

**Note:** If Ionic serve is not working, you can also execute following command (update ports as your wish)

    ionic serve --dev-logger-port 53705 --livereload-port 35740 --port 8300
    
### To generate apk
    ionic cordova platform add android@7.0.0
    ionic cordova build android
Execute `ionic cordova resources` before you build, if you faced any issue with icons or image not found



----


**Common mistakes**

- Update Google API Key with Driver App
- Add Geolocation plugin & whitelist plugin (if it didn't added automatically)
    ```
    ionic cordova plugin add cordova-plugin-geolocation
    ionic cordova plugin add cordova-plugin-whitelist
    ```

If you faced CORS issue, while testing on browser, please run browser without CORS

**Windows:**

    "[PATH_TO_CHROME]\chrome.exe" --disable-web-security --disable-gpu --user-data-dir=~/chromeTemp

**Mac:**
 
    open -n -a /Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome --args --user-data-dir="/tmp/chrome_dev_test" --disable-web-security
