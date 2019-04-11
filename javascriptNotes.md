# Best Practices
## Two ways to avoid Global namespace pollution

1. Declare variables within functions.
2. Declare a single global object, and attach all otherwise global variables to that object.
```
var Vis = {};  //Declare empty global object

Vis.zebras = "still pretty amazing";
Vis.monkeys = "too funny LOL";
Vis.fish = "you know, not bad";
```

# Snippets

## Objects
```
var fruits = [
    {
        kind: "grape",
        color: "red",
        quantity: 12,
        tasty: true
    },
    {
        kind: "kiwi",
        color: "brown",
        quantity: 98,
        tasty: true
    },
    {
        kind: "banana",
        color: "yellow",
        quantity: 0,
        tasty: true
    }
];
```
## GEOJSON
All GeoJSON objects are JSON objects, and all JSON objects are JavaScript objects.

GeoJSON can store points in geographical space (typically as longitude/latitude coordinates), but also shapes (such as lines and polygons) and other spatial features.
```
{
    "type": "FeatureCollection",
    "features": [
        {
            "type": "Feature",
            "geometry": {
                "type": "Point",
                "coordinates": [ 150.1282427, -24.471803 ]
            },
            "properties": {
                "type": "town"
            }
        }
    ]
}
```
```
if (test) {
    // code to run if true
};
```
```
for (var i = 0; i < 5; i++) {
    console.log(i);  //Prints value to console
}
```
