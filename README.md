# jQuery-Google-Place-AutoComplete

## Usage

```html 
<input id="example1" type="text" name="loocation" class="form-control" placeholder="Location"/>

```
```javascript
let locationPicker = $('#example1').LocationRegionPicker({
                    types: '(regions)',
                    map: 'map', // map elemetn id
                    placeChanged: function (place, map) {
                        
                    }
                });
                
```
To get Latitide and longitude
                
```javascript
                 placeChanged: function (place, map) {
                        console.log(place.geometry.location.lat(),place.geometry.location.lng());
                    }
```
