# my-google-locations
This is a Leaflet map visualizing personal location history from Google (Android phone GPS) on OpenStreetMap.  The MarkerCluster plugin for Leaflet is employed due to the significant number of points (avg 2x per minute).

Google location history is in a JSON file you can download from https://takeout.google.com/settings/takeout and needs to be converted to GeoJSON format to work in Leaflet.  There is a Python script to do the conversion here: https://github.com/rtbigdata/google-location-geojson.py  The resulting GeoJSON file can be fairly large, possibly over 100 MB if you've been an Android user for years and always have your GPS enabled.

Live demo using sample data at: https://rtbigdata.github.io/my-google-locations/googletrace.html

This was inspired by Shirin Glander's article on mapping Google location history with R: https://shiring.github.io/maps/2016/12/30/Standortverlauf_post
