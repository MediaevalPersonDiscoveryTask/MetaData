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
- `pointsPosition`: position of some points around the face x1:y1;x2:y2;...xn:yn


## face temporal segmentation (faceSegmentation/video.vtseg)

```
videoID startTime endTime startFrame endFrame personName
```

- `videoID`: unique video identifier
- `startTime`: start time in seconds
- `endTime`: end time in seconds
- `startFrame`: start frame index
- `endFrame`: end frame index
- `personName`: person name (according to convention)


## overlaid names temporal segmentation (OCRSegmentation/video.vtseg)

```
videoID startTime endTime startFrame endFrame personName
```

- `videoID`: unique video identifier
- `startTime`: start time in seconds
- `endTime`: end time in seconds
- `startFrame`: start frame index
- `endFrame`: end frame index
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


## SpeakerSegmentation (SpeakerSegmentation/video.atseg)

```
videoID startTime endTime personName
```

- `videoID`: unique video identifier
- `startTime`: start time in seconds
- `endTime`: end time in seconds
- `personName`: person name (according to convention)


## SpokenSegmentation (SpokenSegmentation/video.atseg)

```
videoID startTime endTime personName
```

- `videoID`: unique video identifier
- `startTime`: start time in seconds
- `endTime`: end time in seconds
- `personName`: person name (according to convention)


