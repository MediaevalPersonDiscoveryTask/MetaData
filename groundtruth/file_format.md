file format
==============

## face position (facePosition/video.position)

```
frameStart endFrame annotatedFrame personName role pointsPosition
```

- `startFrame`: start frame index
- `endFrame`: end frame index
- `annotatedFrame`: frame manually annotated
- `personName`: person name (according to convention)
- `role`: role of the person
- `pointsPosition`: position of some points around the face x1:y1;x2:y2;...xn:yn

## face segmentation (faceSegmentation/video.mdtm)

```
videoID 1 startTime duration head na na personName
```

- `videoID`: unique video identifier
- `startTime`: start time in seconds
- `duration`: duration time in seconds
- `personName`: person name (according to convention)

## OCRSegmentation (OCRSegmentation/video.mdtm)

```
videoID 1 startTime duration written na na personName
```

- `videoID`: unique video identifier
- `startTime`: start time in seconds
- `duration`: duration time in seconds
- `personName`: person name (according to convention)

## Reference (shotAnnotation/video.ref)

```
videoID shotNumber personName isEvidence evidenceSource
```

- `videoID`: unique video identifier
- `shotNumber`: shot number
- `personName`: person name (according to convention)
- `isEvidence`: does this shot provide identity evidence for `personName` (`true`, `false` or `na`)
- `evidenceSource`: `na` or `audio` or `image` or `both` 

## SpeakerSegmentation (SpeakerSegmentation/video.mdtm)

```
videoID 1 startTime duration speaker na na personName
```

- `videoID`: unique video identifier
- `startTime`: start time in seconds
- `duration`: duration time in seconds
- `personName`: person name (according to convention)


## SpokenSegmentation (SpokenSegmentation/video.mdtm)

```
videoID 1 startTime duration spoken na na personName
```

- `videoID`: unique video identifier
- `startTime`: start time in seconds
- `duration`: duration time in seconds
- `personName`: person name (according to convention)


