# Map4D SDK

Map4D SDK for Web, written in Javascript.

[![CocoaPods](https://raw.githubusercontent.com/iotlinkadmin/map4d-web-sdk/master/sdk/map4dweb.png)](https://map4d.vn) 

## Important Changelogs

1. Version 1.2.0

- Use api key for api request

2. Version 1.3.1

- Update location array order: [lat, lng] => [lng, lat]

- Render POI on 2D mode

3. Version 1.4

- Render Tile Overlay

- Render Building Overlay

- Render POI Overlay

## Installation

1. Download map4dsdk from [here](https://github.com/map4d/map4d-web-sdk/blob/master/sdk/map4dsdk%401.4.0.prod.js)


2. Add script to your website
```html
<script src="[PATH]/map4dsdk@[version].js"></script>
```

***Note: SDK script name must contains "map4dsdk@"***

## Using

1. Initialize map with access key

```html
<body>
<div id="map"></div>

<script src="[PATH]/map4dsdk@[version].js"></script>

<script>
  let map = new map4d.Map(document.getElementById("map"),
      {
        center: [105.828042, 21.007651],
        zoom: 17,
        geolocate: true,
        controls :true,
        tilt: 0,        
        accessKey: `${your-key}`
      }
    )
  //set switch mode Auto for automatically switching between 2D & 3D
	map.setSwitchMode(map4d.SwitchMode.Auto)
	map.enable3dMode(true)
</script>

</body>
```

2. Style your view

```css
  <style>
	body {
	  margin: 0px;
	  height: 100%;
	}

	#map {
	  position: absolute;
	  width: 100%;
	  height: 100%;
	  background-color: #f2efe9;
	}
  </style>
  ```

## Document references
[1. Getting started](docs/vi/1.4/0-getting-started.md) 

[2. Map user interaction](docs/vi/1.4/1-map-user-interaction.md) 

[3. Type](docs/vi/1.4/2-type.md)

[4. Map events](docs/vi/1.4/3-map-events.md)

[5. Marker](docs/vi/1.4/4-marker.md)

[6. Marker cluster](https://github.com/iotlinkadmin/map4d-web-sdk/tree/master/docs/vi/1.4/5-marker-cluster.md)

[7. Polyline](docs/vi/1.4/6-polyline.md)

[8. Polygon](docs/vi/1.4/7-polygon.md)

[9. Circle](docs/vi/1.4/8-circle.md)

[10. 3D objects](docs/vi/1.4/9-3d-objects.md)

[11. Tile area](docs/vi/1.4/10-tile-area.md)

[12. Effect](docs/vi/1.4/11-effect-map.md)

[13. LatLngBounds](docs/vi/1.4/12-lat-lng-bounds.md)

[14. Map utils](docs/vi/1.4/13-map-utils.md)

[15. Data layer](docs/vi/1.4/14-data-layer.md)

[16. Leaflet Integrated](docs/vi/1.4/15-leaflet-integrated.md)

[17. Place](docs/vi/1.4/16-place.md)

[18. Tile Overlay](docs/vi/1.4/17-tile-overlay.md)

[19. Building Overlay](docs/vi/1.4/18-building-overlay.md)

[20. POI Overlay](docs/vi/1.4/19-poi-overlay.md)

License
-------

Copyright (C) 2016 IOT Link Ltd. All Rights Reserved.
