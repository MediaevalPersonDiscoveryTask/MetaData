This directory provides additional manual annotations, extracted from the REPERE package.
We provide these files to avoid a potentially painful step of parsing `.trs` and `.xgtf` files.
Because they are under ELRA's usage agreement, these files must be downloaded separately from the password-protected PBWorks wiki: http://mediaeval15.pbworks.com/w/file/96099734/dev.manual.20150508.tgz

* `speaker`

 This directory provides manual annotations in speaker (who speaks when). Each file contains one line per speech turn, using [`.MESeg` file format](https://github.com/MediaevalPersonDiscoveryTask/metadata/wiki/file-format#temporal-segmentation-meseg).

* `facetrack`

 This directory provides manual annotations in faces (who appears when). Each file contains one line per face track, using [`.MESeg` file format](https://github.com/MediaevalPersonDiscoveryTask/metadata/wiki/file-format#temporal-segmentation-meseg).

* `written`

 This directory provides manual annotations of overlaid person names. Each file contains one line per person name occurrence (with start and end times), using [`.MESeg` file format](https://github.com/MediaevalPersonDiscoveryTask/metadata/wiki/file-format#temporal-segmentation-meseg).

* `spoken`

 This directory provides manual annotations of uttered person names. Each file contains one line per person name occurrence (with start and end times), using [`.MESeg` file format](https://github.com/MediaevalPersonDiscoveryTask/metadata/wiki/file-format#temporal-segmentation-meseg).

* `face_position`
  
 This directory provides manual annotations for face detection. Each file contains one line per annotated frame (not all frames were annotated in the REPERE dataset), using [`.position` file format](https://github.com/MediaevalPersonDiscoveryTask/metadata/wiki/file-format#face-position-position).
 
