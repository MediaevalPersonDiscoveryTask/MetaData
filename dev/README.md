
## Development set

* `subsets`

 The development set was used during REPERE evaluation campaigns in 2012 (evaluation `0`), 2013 (evaluation `1`) and 2014 (evaluation `2`), and is therefore divided into several subsets (`dev0`/`test0`, `dev1`/`test1` and `dev2`/`test2`) described in `SUBSET.lst` files providing the corresponding list of `videoID`.

* `dataPath.lst`

 This file has one line per video in the REPERE corpus.
 It provides path to several resources, relative to directory `REPERE/DATA/SOURCE DATA/` on development set hard drive.

 ```
 videoID wav avi mpg trs xgtf idx
 ```

 - `videoID`: video identifier
 - `wav`: path to `.wav` file
 - `avi`: path to `.avi` file
 - `mpg`: path to `.mpg` file
 - `trs`: path to [`.trs` file](https://github.com/MediaevalPersonDiscoveryTask/metadata/wiki/file-format#transcriber-trs)
 - `xgtf`: path to [`.xgtf` file](https://github.com/MediaevalPersonDiscoveryTask/metadata/wiki/file-format#viper-xgtf)
 - `idx`: path to [`.idx` file](https://github.com/MediaevalPersonDiscoveryTask/metadata/wiki/file-format#video-index-idx)


* `dev.uem`
 
 Only parts of the REPERE corpus were manually annotated. 
 This file provides the list of those parts using [`.uem` file format](https://github.com/MediaevalPersonDiscoveryTask/metadata/wiki/file-format#unpartitioned-evaluation-map-uem).

* `groundtruth`

 This directory provides label and evidence groundtruth in [`SUBSET.ref`](https://github.com/MediaevalPersonDiscoveryTask/evaluation/wiki/File-format#reference-ref) and [`SUBSET.eviref`](https://github.com/MediaevalPersonDiscoveryTask/evaluation/wiki/File-format#evidence-reference-eviref) respectively. 

* `submission_shot`

 This directory provides the filtered output of automatic segmentation into shots in [`SUBSET.shot` files](https://github.com/MediaevalPersonDiscoveryTask/evaluation/wiki/File-format#shots-shot).
 Submission files on a given `SUBSET` must report results for these shots only.
 It means that evidences must also be searched among these shots, and only among these shots.
 See `automatic` for the complete list of shots, if you feel like it might be useful.

* `manual`

 This directory provides additional manual annotations, extracted from the REPERE package. We provide these files to avoid a potentially painful step of parsing `.trs` and `.xgtf` files. Because they are under ELRA's usage agreement, these files must be downloaded separately from the password-protected PBWorks wiki: http://mediaeval15.pbworks.com/w/file/96099734/dev.manual.20150508.tgz

* `automatic`

  This directory provides the output of several automatic processing modules (optical character recognition, speaker diarization, face tracking, talking-face detection, etc.).
  You can expect these files to also be available for the test set in June.
  This means that you can rely on these files for developping your algorithms in case you do not have expertise in all involved research fields. 

* `baseline`

  This directory provides the submission files of the baseline system whose source code is available [here](https://github.com/MediaevalPersonDiscoveryTask/baseline).
