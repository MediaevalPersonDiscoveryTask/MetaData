
WORK IN PROGRESS - WORK IN PROGRESS - WORK IN PROGRESS - WORK IN PROGRESS

Metadata are being generated on a subset of the development dataset right now.  
Announcement will be sent to the mailing-list when they are ready (expected deadline: May 8th).

WORK IN PROGRESS - WORK IN PROGRESS - WORK IN PROGRESS - WORK IN PROGRESS


## Development set

* `dev/subsets`

 The development set was used during REPERE evaluation campaigns in 2012 (evaluation `0`), 2013 (evaluation `1`) and 2014 (evaluation `2`), and is therefore divided into several subsets (`dev0`/`test0`, `dev1`/`test1` and `dev2`/`test2`) described in `SUBSET.lst` files providing the corresponding list of `videoID`.

* `dev/groundtruth`

 This directory provides label and evidence groundtruth in `SUBSET.ref` and `SUBSET.eviref` respecively. 

* `dev/submission_shot`

 This directory provides the filtered output of automatic segmentation into shots in `SUBSET.shot` files.  
 Submission files on a given `SUBSET` must report results for these shots only.  It means that evidences must also be searched among these shots, and only among these shots.  
 See `dev/automatic` for the complete list of shots, if you feel like it might be useful.

* `dev/manual`

* `dev/automatic`

* `dev/baseline`


