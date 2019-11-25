Florence 3D actions dataset

The dataset collected at the University of Florence during 2012, has been captured using a Kinect camera. It includes 9 activities: wave, drink from a bottle, answer phone,clap, tight lace, sit down, stand up, read watch, bow. During acquisition, 10 subjects were asked to perform the above
actions for 2/3 times. This resulted in a total of 215 activity samples.
We suggest a leave-one-actor-out protocol: train your classifier using all the sequences from 9 out of 10 actors and test on the remaining one. Repeat this procedure for all actors and average the 10 classification accuracy values.


Videos depicting the actions are named GestureRecording_Id<ID_GESTURE>actor<ID_ACTOR>idAction<ID_ACTION>category<ID_CATEGORY>.avi
The file The file Florence_dataset_Features.txt contains all the pose features with annotate actor and actions. Each line is formatted according to the following:

%idvideo idactor idcategory  f1....fn

where f1-f24 are our normalized body part coordinates
and f25 is the normalized frame value.

Specifically:

elbows: f1-f6; (1-3 left elbow, 4-6 right elbow, same applies for all other joints)
wrists: f13-f18
knees: f7-f12
ankles: f19-f24
normalized frame value: f25



The file Florence_dataset_WorldCoordinates.txt
Contains the world coordinates for all the joints. Thanks to Maxime Devanne for parsing this data! Each line is formatted according to the following:

%idvideo idactor idcategory  f1....fn
where f1-f45 are world coordinates of all the 15 joints.

Specifically:
Head: f1-f3
Neck: f4-f6
Spine: f7-f9
Left Shoulder: f10-f12
Left Elbow: f13-f15
Left Wrist: f16-f18
Right Shoulder: f19-f21
Right Elbow: f22-f24
Right Wrist: f25-f27
Left Hip: f28-f30
Left Knee: f31-f33
Left Ankle: f34-f36
Right Hip: f37-f39
Right Knee: f40-f42
Right Ankle: f43-f45




 

