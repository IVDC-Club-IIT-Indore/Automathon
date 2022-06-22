


# **Automathon 2022**

TASKS: 

1.1   
- Object Detection( a) Cars and b) Bikes in the Video)

1.2
- Lane Detection

Bonus 
- Object Tracking (Bonus ) and Counting( extra from my side)




## 1.1. a)Cars detection & b) Bikes detection


I have used the YOLOv5 algorithm  for object detection for the given input video.
Taken help from the following sources: 
guide: https://docs.ultralytics.com/quick-start/
reference video : https://github.com/ultralytics/yolov5


 RESULTS: https://drive.google.com/file/d/1zimiVEmHrjT0--5r-wJQ38Sk2NS7VSUR/view?usp=sharing



*NOTE:* I understand the fact that YOLOv4 could have been the better choice wrt accuracy ,but due to some compatibility(most probably) issues , I wasn't able to complete that model using YOLOv4 but instead used YOLOv5     https://arxiv.org/pdf/2004.10934v1.pdf



## 1.2   	 Lane Detection
In this part I have used :

- Camera Calibration -remove the curved line related errors present in video
- Thresholding -  converting image to binary using some threshold value (To differenciate the lanes from surrounding)
- Perspective transformation ( considering the lanes to be going farther and thereby deciding the lines trapezoid like thing is actually a rectangle) 
- LaneLines ( identifying the lane lines)
- etc
 
 RESULTS: https://drive.google.com/file/d/1NdFZXxhFd9rXld62VRMdMql_XiXXXEMR/view?usp=sharing

references
https://github.com/Dt-Pham/Advanced-Lane-Lines.git
https://www.youtube.com/watch?v=iRTuCYx6quQjec

## Bonus

## Object Tracking(Given )

readings: https://viso.ai/deep-learning/object-tracking/

In that process I actually Solved a bug in the code, from the reference repository  I  was refering to ( basically the module it was using was outdated)
https://stackoverflow.com/questions/62390517/no-module-named-sklearn-utils-linear-assignment

Attempted in the following manner :
-used open cv  based methods for object tracking

## Object Counting(extra from my side)
Added along with Tracker( My attempt for counting vehicles seems a lot inaccurate , I am trying to improve on it)

https://github.com/guptavasu1213/Yolo-Vehicle-Counter/blob/master/README.md
https://github.com/bamwani/car-counting-and-speed-estimation-yolo-sort-python/blob/master/README.md


