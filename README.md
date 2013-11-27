Based on a [DGPlayer Fork](https://github.com/audiocogs/dgplayer) combined with [audiocogs aurora](https://github.com/audiocogs/aurora.js) with [FLAC](https://github.com/audiocogs/flac.js) and [MP3](https://github.com/audiocogs/mp3.js)

Pure javascript, [underscore](http://underscorejs.org/#template) is used for templating the playlist

### Playlist usage

Just pass into `DGPlayer.playist` an array of songs :

```
    DGPlayer.playlist = [
    						{name : "Song1 name", url : "http://localhost/media/mySong.mp3"}, 
    						{name : "Song2 name", url : "http://localhost/media/mySong.flac"}
    					];
```

### Album usage

If you want to play an album, just pass artist, album and cover to `DGPlayer.album` :

```
    DGPlayer.album = {artist : 'Artist', album : 'Album', picture : 'http://localhost/img/avatar.jpeg'};
```

You might also set the playlist through the album by adding songs :

```
    DGPlayer.album = {
    					artist : 'Artist', 
    					album : 'Album', 
    					picture : 'http://localhost/img/avatar.jpeg', 
    					songs : [
    						{name : "Song1 name", url : "http://localhost/media/mySong.mp3"}, 
    						{name : "Song2 name", url : "http://localhost/media/mySong.flac"}
    					]
    				};

```

### Todo

Add/remove song method

Built for [ezseed2](github.com/soyuka/ezseed2)