# Switzerland cantons and communes

## Source

For Cantons and Communes: OpenStreetMap extract from Mapzen
https://mapzen.com/data/borders/

For lakes: OpenStreetMap extract with Overpass turbo http://overpass-turbo.eu/

For peaks: Wikipedia https://en.wikipedia.org/wiki/List_of_mountains_of_Switzerland#Main_list

## Fixes

* Inconsistencies in data (some cantons and communes include lakes, some don't. Now all are without lakes)
* Added missing communes Erlen and Sulgen

## Files

The **canton_id** and **commune_id** correspond to those used by [Swiss statistics](http://www.bfs.admin.ch/bfs/portal/en/index.html). The **abbrev** property in cantons.json is a two letter abbreviation such as used on license plates.

### cantons.json

Properties: 
* name (Name in local language(s))
* name_de
* name_fr
* name_it
* iso (ISO3166-2)
* canton_id
* abbrev

### communes.json

Properties:
* name
* shn (created from canton_id, district_id and commune_id)
* canton_id
* commune_id

### lakes.json

Major lakes

Properties:
* name (Name in local language(s))
* name_de
* name_fr
* name_it

### peaks.json

Properties:
* alt
* rank
* name

## Simplified files

* cantons_1%.json
* communes_1%.json
* lakes_1%.json

Simplified with [mapshaper](http://mapshaper.org/)

