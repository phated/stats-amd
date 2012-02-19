### Usage ###

```javascript
require([ 'Stats' ], function ( Stats ) {
  var stats = new Stats();

  // Align top-left
  stats.getDomElement().style.position = 'absolute';
  stats.getDomElement().style.left = '0px';
  stats.getDomElement().style.top = '0px';

  document.body.appendChild( stats.getDomElement() );

  setInterval( function () {

    stats.update();

  }, 1000 / 60 );
});
```
