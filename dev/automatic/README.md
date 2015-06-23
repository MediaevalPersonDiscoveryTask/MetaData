
## Automatic processing

* `raw_shot`

 This directory provides the raw output of automatic segmentation into shots in [`SUBSET.shot` files](https://github.com/MediaevalPersonDiscoveryTask/evaluation/wiki/File-format#shots-shot).
 This is **NOT** the list of shots that must be used for submission.
 It is just here for convenience in case you need a complete set of shots.

* `speaker`

 This directory provides the output of automatic speaker diarization (who speaks when). 
 Each file contains one line per speech turn, using [`.MESeg` file format](https://github.com/MediaevalPersonDiscoveryTask/metadata/wiki/file-format#temporal-segmentation-meseg). 

* `speechturn_similarity`

 This directory provides probabilities that each speech turn correspond to an other speech turn.

 ```
trackIDspeechTurn trackIDspeechTurn probability
 ```

* `facetrack`

 This directory provides automatic face detection and tracking. Each file contains one line per face track, using [`.MESeg` file format](https://github.com/MediaevalPersonDiscoveryTask/metadata/wiki/file-format#temporal-segmentation-meseg).

* `facetrackPosition.tar.gz`

 This archive contain the position of facetracks. Each file contain one line per frame/facetrack, using 
 
 ```
frameID faceTrackID xmin, ymin, width, height
 ```

* `face`

 This directory provides the output of automatic face track clustering. Each file contains one line per face track, using [`.MESeg` file format](https://github.com/MediaevalPersonDiscoveryTask/metadata/wiki/file-format#temporal-segmentation-meseg).

* `facetrack_similarity`

 This directory provides matrix probability that two faces correspond to the same person. 
 Due to the size of the files, they must be downloaded separately from the PBWorks wiki:
 http://mediaeval15.pbworks.com/w/file/96824115/facetrack_similarity.tgz

* `speakingface`

 This directory provides probabilities that each face track correspond to the current speaker. Each file contains one line per overlapping (face track / speech turns).

 ```
trackIDspeechTurn trackIDfaceTrack probability
 ```

* `written`

 This directory provides automatic detection of overlaid person names. Each file contains one line per person name occurrence (with start and end times), using [`.MESeg` file format](https://github.com/MediaevalPersonDiscoveryTask/metadata/wiki/file-format#temporal-segmentation-meseg).

* `ASR`

 This directory provides the raw output of an automatic speech recogntion system

 ```
videoID 1 startTime endTime word confidence
 ```

* `spoken`

 This directory provides the raw output of an automatic named entites detection in ASR, using [`.MESeg` file format](https://github.com/MediaevalPersonDiscoveryTask/metadata/wiki/file-format#temporal-segmentation-meseg).

