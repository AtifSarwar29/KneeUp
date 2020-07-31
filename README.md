# KneeUp
This project analyze the knee up skeleton data to check the knee fitness of people.
## OpenPose Skeleton Keypoints
- run the command to get the json files, images and video of skeleton keypoints by OpenPose
```
./build/examples/openpose/openpose.bin --model_pose BODY_21A --tracking 1 --render_pose 1 --video input-video-folder-path/video.avi --write_video output-video-folder-path/nol22.avi --write_images output-json-folder-path --write_json output-json-folder-path --display 0
```
## Track the person by the mean of skeleton keypoints
To track people in skelton json files run the command  

- change the json directory path

```
python TrackSkeletonSequence.py
```

## Analysis Skeleton keypoints data 
-run the command to analsis the skelton json to get the maximum angle, excel file for result 

- change the path to input  for track json directory 
- change path to save excel file directory 
- change the path for skeleton images directory

```
python KneeUpAnalysis.py
```


## Video generation

- change skelton image directory to put text on images
- change the path to save video file

```
python Video-Generate.py
```
