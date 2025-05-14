# River walks

River walks!

How to get data, from [weeknote 2024/29](https://weeknotes.alifeee.co.uk/2024-29/).

```text
Here is the River Sheaf on Open Street Map (OSM)

<https://www.openstreetmap.org/relation/11890887>

It is made up of a series of "ways", which are lines with coordinates, added by normal people.

I used Overpass Turbo (<https://overpass-turbo.eu/s/1OyD>) to export a [`geoJSON`](https://geojson.org/) file for the River Sheaf (i.e., with `relation(11890887); out geom;`)

to crop:

sudo apt install gdal-bin
ogr2ogr -clipsrc -1.47927 53.34511 -1.49590 53.35812 export2.geojson export.geojson
```
