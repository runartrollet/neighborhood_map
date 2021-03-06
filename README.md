# Neighborhood-map

This is a project assigned by Udacity.

#### Highlighted features:
- Single page application
- Big map with muliple preselected locations.
- See weatherinformaion from current location in the map.
- Retrieve and locate nearby restaurants.
- Custom markers.

You can preview the application here:

<h2 style="color: #1d2a61">
<a href="https://neighborhood-map-runar.herokuapp.com/">Neighborhood-map-runar.herokuapp.com</a>

</h2>

## Attribution
Weather data collected from <a href="http://www.darksky.net">DarkSky.net</a>

Restaurant-info collected from <a href="http://www.yelp.com">Yelp.com</a>

Map by <a href="http://maps.google.com">Google Maps</a>

Built with <a href="http://getbootstrap.com">Bootstrap</a>, <a href="http://knockoutjs.com">Knockout</a> and <a href="http://jquery.com">jQuery</a>
</p>
<p>App built by <a href="http://runarkristoffersen.com/">Runar Kristoffersen</a>, >as part of an assignment in the <a href="https://www.udacity.com/course/full-stack-web-developer-nanodegree--nd004">Full-Stack course at Udacity</a>.</p>

# Getting up and running

This project uses python3.

To install the required packages, do this:
```
pip install -r requirements.txt
```
## Setting config-parameters

You need to provide some basic configuration, like database-name for PSQL, client_id and client_secret.

You have two choices for how you wish to set these config-parameters, of which only one is required.

### Option 1. Store them in a file
Create a file `instance/config.cfg`.

the contents of this file shuld be in this format:
```
TESTING=False
DEBUG=True
YELP_CLIENT_ID="YOUR CLIENT ID HERE"
YELP_CLIENT_SECRET="YOUR CLIENT SECRET HERE"
```

### Option 2. OS-envirnment variables.
```
export YELP_CLIENT_ID=YOUR CLIENT ID HERE
export YELP_CLIENT_SECRET=YOUR CLIENT SECRET HERE
```

## Initiate default-database

After you have created that file, you can run this command to generate the  database-structure, and insert some default-data. Note that the database itself will have to be created in advance.
```
python app.py --setup
```

## Running the app
```
python app.py
```
