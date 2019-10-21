# Creating Google MAps Api Key

We have used google maps api for displaying maps, calculating distance, markers ..etc. so we need to create google maps api key & update required files before starting remaining setup.

### Create new project

- Login to https://console.developers.google.com/projectcreate with your google account
- create new project

![create-new-project]( https://github.com/codesundar/ionic-uber-clone/blob/master/img/create-new-project.png "create-new-project")

### Create API key

- Navigate to your currect project & goto to API settings https://console.developers.google.com/apis/dashboard
- Goto Credenitals & Create New API Key

![create-api-key]( https://github.com/codesundar/ionic-uber-clone/blob/master/img/create-api-key.png "create-api-key")

Once you created API key, you need to update with following files

- Driver/src/index.html
- Rider/src/index.html

### Enabling required services

- Navigate to library & choose google maps (view all)
- enable all Required API's
    - Direction
    - Distance Matrix
    - Geocoding
    - Geolocation
    - Maps Embed
    - Maps JavaScript
    - Maps Places (aka Places API)

![enable-map-api]( https://github.com/codesundar/ionic-uber-clone/blob/master/img/enable-map-api.png "enable-map-api")


**Important Update:** Google Maps free API allows only one request / min. So must verfiy your credit card with Google Billing (https://console.developers.google.com/billing/) to avoid these errors.

Please visit for more info: https://cloud.google.com/maps-platform/pricing/


### What you did ?
- Created Google Project
- Created API key
- Enabled all required services
- Added Google Billing (optional)
- Updated API key on driver & rider files
