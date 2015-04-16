file format
==============

## uri list (.lst)

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

## trs (.trs)

Audio manual annotation (speaker identity and speech transcription) in the Transcriber format

## xgtf (.xgtf)

Video annotation (face position, overlaid text transcription) in XGTF format (Viper)

## idx (.MPG.idx)

Indexes of the video files, to convert frame number of the video.avi read with opencv to timestamp

```
frameID typeFrame positionInTheVideo timestamp
```

- `frameID`: frame number of the video.avi read with opencv
- `typeFrame`: `I` or `B` or `P` 
- `positionInTheVideo`: position in octet in the video file
- `timestamp`: corresponding timestamp

## Shot List (.shot)

```
videoID shotNumber startTime endTime startFrame endFrame
```

- `videoID`: unique video identifier
- `shotNumber`: shot number
- `startTime`: start time in seconds
- `endTime`: end time in seconds
- `startFrame`: start frame index
- `endFrame`: end frame index

## Video_OCR (.mdtm)


## ASR


## Spoken_name (.mdtm)


## SpeechTurn_segmentation (.mdtm)


## Speaker_diarization (.mdtm)


## Face_segmentation (.mdtm)


## SpeakingFace_segmentation (.mdtm)


## Face_clustering (.mdtm)


## SpeakingFace_clustering (.mdtm)


## SpeechTurn_Face_clustering (.mdtm)


## SpeechTurn_SpeakingFace_clustering (.mdtm)


## Distance_SpeechTurn_vs_SpeechTurn (.mat)
<video> <SpeechTurn> <SpeechTurn> <distance>

## Distance_Face_vs_Face (.mat)
<video> <Face> <Face> <distance>


## Distance_SpeakingFace_vs_SpeakingFace (.mat)
<video> <SpeakingFace> <SpeakingFace> <distance>


## Distance_SpeechTurn_vs_SpeakingFace (.mat)
<video> <SpeechTurn> <SpeakingFace> <distance>
