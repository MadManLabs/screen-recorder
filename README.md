# Screen recorder

OS X screen recording library for Node

## Installation

```
npm install screen-recorder
```

## Example

```
var ScreenRecorder = require('screen-recorder')
var path = require('path')

var movie = new ScreenRecorder(path.resolve(__dirname, 'test.mp4'))
movie.setCapturesMouseClicks(true)
movie.setCropRect(0, 0, 500, 500)
movie.start()

setTimeout(function() {
  movie.stop()
}, 10000)
```
