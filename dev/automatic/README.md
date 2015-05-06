
## Automatic processing

* `raw_shot`

 This directory provides the raw output of automatic segmentation into shots in [`SUBSET.shot` files](https://github.com/MediaevalPersonDiscoveryTask/evaluation/wiki/File-format#shots-shot).
 This is **NOT** the list of shots that must be used for submission.
 It is just here for convenience in case you need a complete set of shots.

* `speaker`

 This directory provides automatic speaker diarization (who speaks when). 
 Each file contains one line per speech turn, using [`.MESeg` file format](https://github.com/MediaevalPersonDiscoveryTask/metadata/wiki/file-format#temporal-segmentation-meseg). 

* `facetrack`

 This directory provides automatic face detection and tracking. Each file contains one line per face track, using [`.MESeg` file format](https://github.com/MediaevalPersonDiscoveryTask/metadata/wiki/file-format#temporal-segmentation-meseg).

* `speakingface`

 This directory provides probabilities that each face track correspond to the current speaker. Each file contains one line per overlapping (face track / speech turns).

 ```
speechTurnID faceTrackID probability
 ```

* `written`

 This directory provides automatic detection of overlaid person names. Each file contains one line per person name occurrence (with start and end times), using [`.MESeg` file format](https://github.com/MediaevalPersonDiscoveryTask/metadata/wiki/file-format#temporal-segmentation-meseg).

