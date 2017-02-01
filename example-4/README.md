## Example 4

This example includes both a Mapbox background vector tile layer, and an uploaded dataset converted into vector tiles with Mapbox Studio.

## Usage
1. Open the file `vektor101/example-4/example-4.html` in your browser.
2. Zoom in and out to see different features appear and disappear.
3. Open the file `example-4.html` in your text editor, and see the comments for how to change styles.

<img width="446" alt="screen shot 2017-02-01 at 16 36 12" src="https://cloud.githubusercontent.com/assets/2197944/22513465/9b020c3e-e89c-11e6-95ac-ccecc85fdfdf.png">

## How to upload your own datasets
1. Create free account on [Mapbox Studio](https://www.mapbox.com/studio/)
2. Upload a new dataset: Click on "New Dataset" on [this page](https://www.mapbox.com/studio/datasets/), then the "Upload" tab. Upload your `.geojson` file, name your Dataset and click "Create". ![upload-mapbox](https://cloud.githubusercontent.com/assets/2197944/22513901/ec719e44-e89d-11e6-8f94-db42e9731354.gif)
3. Convert your dataset to a `Tileset` and get the `tileset` ID (for example 'mapic.ciyn4c1wa004r32ljcrxlmdbb-5onk0')
4. Exchange the source in the example with your new tileset. ```javascript
 "source": {
    type: 'vector',
    url: 'mapbox://YOUR-TILESET-ID'
},
```
5. Then you can change style (fill, line, etc) to fit your `.geojson` data (linestring, polygon). 
6. Refresh the page, and your data should be visible. Then play around some more! :)