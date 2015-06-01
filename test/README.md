
## Test set

* `subsets`

 The test set is coming from the french channel `France 2`. It contains 172 videos of TV news. The list of `videoID` can be found in the file `all.lst`


* `submission_shot`

 This directory provides the filtered output of automatic segmentation into shots in [`SUBSET.shot` files](https://github.com/MediaevalPersonDiscoveryTask/evaluation/wiki/File-format#shots-shot).
 Submission files on a given `SUBSET` must report results for these shots only.
 It means that evidences must also be searched among these shots, and only among these shots.
 See `automatic` for the complete list of shots, if you feel like it might be useful.

* `automatic`

  This directory provides the output of several automatic processing modules (optical character recognition, speaker diarization, face tracking, talking-face detection, etc.).
  You can expect these files to also be available for the test set in June.
  This means that you can rely on these files for developping your algorithms in case you do not have expertise in all involved research fields. 

* `baseline`

  This directory provides the submission files of the baseline system whose source code is available [here](https://github.com/MediaevalPersonDiscoveryTask/baseline).
