# canvas-orbit-camera [![experimental](http://badges.github.io/stability-badges/dist/experimental.svg)](http://github.com/badges/stability-badges)

An alternative wrapper for
[orbit-camera](http://github.com/mikolalysenko/orbit-camera) that works
independently of [game-shell](http://github.com/mikolalysenko/game-shell).

Controls are as follows:

* Rotate - Left click
* Pan - Right click or Control + Left click
* Zoom - Scroll or Shift + Left click

Based heavily on
[game-shell-orbit-camera](http://github.com/mikolalysenko/game-shell-orbit-camera).

## Usage

[![NPM](https://nodei.co/npm/canvas-orbit-camera.png)](https://nodei.co/npm/canvas-orbit-camera/)

### camera = createCamera(canvas)

Attaches a modified `orbit-camera` instance to the `canvas` – attaching the
required event listeners for interaction.

See the [orbit-camera documentation](https://github.com/mikolalysenko/orbit-camera#readme)
for a full list of available methods.

### camera.tick()

Call this at the beginning of each frame to update the current position of the
camera.

### camera.view([out])

Returns the current view matrix associated by the camera: a 16-element (4x4)
`Float32Array` instance. Optionally, you can pass in your own array `out` here
too.

## License

MIT. See [LICENSE.md](http://github.com/hughsk/canvas-orbit-camera/blob/master/LICENSE.md) for details.
