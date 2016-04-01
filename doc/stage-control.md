# StageControl

## usage

```js
var stage = stg.StageControl(options);

stage.on("spawnenemy", function(e) {
  var enemy = e.EnemyClass();
  enemy.addChildTo(scene.enemyLayer);
});

stage.addChildTo(scene);
```

## options

```js
var options = {
  viewport: {
    width: 640,
    height: 960,
  },
  data: {
    enemySpawners: [{
      className: "mygame.Enemy1",
      x: 0,
      y: 0,
    }, {
      className: "mygame.Enemy1",
      x: 0,
      y: 0,
    }, ],
    objectSpawners: [],
  },
  cameraRoute: [
    { x: 320, y: 9120, },
    { x: 320, y: 480, },
  ],
  timeline: [
    { type: "set", cameraSpeed: "5", },
  ],
};
```
### options.viewport

### options.data

## event

### spawnenemy

### spawnobject
