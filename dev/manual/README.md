file format
==============

## Mediaeval segmentation (.MESeg)

```
videoID startTime endTime startFrame endFrame trackID personName confidence
```

- `videoID`: unique video identifier
- `startTime`: start time in seconds
- `endTime`: end time in seconds
- `startFrame`: start frame index
- `endFrame`: end frame index
- `trackID`: unique identifier of the track
- `personName`: person name (according to convention)
- `confidence`: confidence

### face temporal segmentation (faceSegmentation/videoID.MESeg)

Temporal segmentation of the faces appearing in the annotated frames

### overlaid names temporal segmentation (OCRSegmentation/videoID.MESeg)

Temporal segmentation of the overlaid names appearing in the annotated frames

### SpeakerSegmentation (SpeakerSegmentation/videoID.MESeg)

Temporal speakers segmentation in the uem parts

### SpokenSegmentation (SpokenSegmentation/videoID.MESeg)

Temporal segmentation of the pronounced names in the uem parts


## face position (facePosition/videoID.position)

Position of the faces in the annotated frames

```
annotatedFrame trackID personName pointsPosition
```

- `annotatedFrame`: frame manually annotated
- `trackID`: unique identifier of the track
- `personName`: person name (according to convention)
- `pointsPosition`: position of some points around the face x1:y1;x2:y2;...xn:yn

