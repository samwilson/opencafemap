OpenCaféMap
===========

This is a map of cafés.

## Overpass Turbo query

For http://overpass-turbo.eu/

```
[out:json][timeout:25];
(
  node["amenity"="cafe"]({{bbox}});
  way["amenity"="cafe"]({{bbox}});
  relation["amenity"="cafe"]({{bbox}});
);
out body;
>;
out skel qt;
```
