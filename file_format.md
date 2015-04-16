file format
==============

## uri list (uri_lst/uri.set.lst)

```
videoID\twaveFile\tvideoAVIFile\tvideoMPEGFile\ttrsFile\txgtfFile\tidxFile
```

- `videoID`: unique video identifier
- `waveFile`: path to the videoID.wav file
- `videoAVIFile`: path to the videoID.avi file
- `videoMPEGFile`: path to the videoID.MPG file
- `trsFile`: path to the videoID.trs file
- `xgtfFile`: path to the videoID.xgtf file
- `idxFile`: path to the videoID.MPEG.idx


## trs (video.trs)

Audio manual annotation (speaker identity and speech transcription) in the Transcriber format


## xgtf (video.xgtf)

Video annotation (face position, overlaid text transcription) in XGTF format (Viper)


## idx (video.MPG.idx)

Indexes of the video files, to convert frame number of the video.avi read with opencv to timestamp

```
frameID typeFrame positionInTheVideo timestamp
```

- `frameID`: frame number of the video.avi read with opencv
- `typeFrame`: `I` or `B` or `P` 
- `positionInTheVideo`: position in octet in the video file
- `timestamp`: corresponding timestamp


## Shot List (shotSegmentation/video.shot)

```
videoID shotNumber startTime endTime startFrame endFrame
```

- `videoID`: unique video identifier
- `shotNumber`: shot number
- `startTime`: start time in seconds
- `endTime`: end time in seconds
- `startFrame`: start frame index
- `endFrame`: end frame index

