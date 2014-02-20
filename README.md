*This repository is a mirror of the [component](http://component.io) module [stagas/mod-player](http://github.com/stagas/mod-player). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/stagas-mod-player`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# mod-player

module (.mod) player in javascript

## Example

```js
function play(buffer){
  if (playing) playing.disconnect();
  var mod = new ModParser(buffer);
  var player = new ModPlayer(mod, audio.sampleRate);
  var node = playing = process(audio, sampleLength, player.process);
  node.connect(audio.destination);
}
```

## Credits

* [gasman](https://github.com/gasman) [original](https://github.com/gasman/jsmodplayer)
* [BillyWM](https://github.com/BillyWM) [improvements (fork based upon)](https://github.com/BillyWM/jsmodplayer)

## License

MIT
