This directory provides matrix probability that two faces correspond to the same person.
Due to the size of the files, they must be downloaded separately from the PBWorks wiki: 
http://mediaeval15.pbworks.com/w/file/96919803/test.facetrack_similarity.tgz

Here is an example of how to read these matrices in Python: 

```python
from mediaeval_util.repere import MESegParser
import pickle
from scipy import spatial

# read face segmentation
TrackFaceIDs = []
face_seg, confs, timeToFrameID = MESegParser(args['<faceTrackSegmentation>'], args['<videoID>'])
for s, t, l in face_seg.itertracks(label=True):
    TrackFaceIDs.append([t, l])
TrackFaceIDs.sort()

# read matrix
mat = pickle.load(matrix_file, "rb" ))
mat = spatial.distance.squareform(mat, checks=False)

# print the similarity of two facetracks
for i in range(len(TrackFaceIDs)):
    for j in range(len(TrackFaceIDs)):
        print TrackFaceIDs[i], TrackFaceIDs[j], mat[i][j]
```
