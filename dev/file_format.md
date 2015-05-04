file format
==============

## data path (dataPath.lst)

Path to the different ressources for an videoID (in the folder `REPERE/DATA/SOURCE DATA/` for the REPERE corpus)

```
videoID waveFile videoAVIFile videoMPEGFile trsFile xgtfFile idxFile
```

- `videoID`: unique video identifier
- `waveFile`: path to the videoID.wav file
- `videoAVIFile`: path to the videoID.avi file
- `videoMPEGFile`: path to the videoID.MPG file
- `trsFile`: path to the videoID.trs file
- `xgtfFile`: path to the videoID.xgtf file
- `idxFile`: path to the videoID.MPEG.idx


## uri list (uri_lst/uri.set.lst)

```
videoID
```

- `videoID`: unique video identifier


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

## Reference (.ref)

```
videoID shotNumber personName
```

- `videoID`: unique video identifier
- `shotNumber`: shot number
- `personName`: person name (according to convention)

## Evidence reference (.eviref)

```
videoID shotNumber personName evidenceSource
```

- `videoID`: unique video identifier
- `shotNumber`: shot number
- `personName`: person name (according to convention)
- `evidenceSource`: `audio` or `image` or `both` 


