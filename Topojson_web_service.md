# Topojson web service

Status: Partially claimed!  ITOS making the service for a few countries.  Need to think about other countries.

Overview
ITOS are releasing geometry files for country and their sub boundaries with pcodes.  Unfortunately these data sets are far too high resolution and heavy formats to be used in web applications.  This app aims to pull the latest data from ITOS, reduce the resolution and convert to topojson so that it can be used in webapps.

ITOS Data
https://public.tableau.com/profile/hernusi#!/vizhome/COD-Status/UsabilityEvaluationOverview

Daily script will check for updates to geometries or new countries added.  If there are news ones it will download the file, simplify the geometry and convert to topojson

An api is then built to query against with for example:

/SLE/2

Which return Sierra Leone adm2 as a simplified topojson.
