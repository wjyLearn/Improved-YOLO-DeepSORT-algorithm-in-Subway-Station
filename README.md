We optimized and combined the YOLOv8 detection model and DeepSORT tracking algorithm, and applied it to the passenger flow statistics of subway stations to achieve real-time statistics of passenger flow count, speed and density at key locations. The passenger flow information obtained can help the management department to adjust the operation strategy in time, ensure the safety of the station and improve the operation efficiency.


# Yolov8
Based on the improvement of YOLOv8 network, the output module with high dimensional features is removed in Head layer to simplify the model. A new fusion module is added in the Neck layer to fully integrate the feature information of different scales. CBAM attention mechanism is added to Backbone layer to enhance the extraction of useful feature information.

https://github.com/wjyLearn/Improved-YOLO-DeepSORT-algorithm-in-Subway-Station/blob/main/YOLOv8.png

# DeepSORT
The tracking strategy of DeepSORT algorithm is optimized. Headshoulder dataset was used to train ReID model, which alleviated the problem of frequent ID switching when only pedestrian head and shoulder were detected and tracked in subway applications. According to the motion state of passenger flow in the subway scene, the tracking area is delimited to reduce the redundant detection objects passed into the tracker, and the failed tracks in the tracker are deleted in time, so as to reduce the calculation amount during the matching calculation of the tracking algorithm and accelerate the processing speed of the algorithm. Compared with the original algorithm, the processing speed of the optimized tracking algorithm is increased by 45%, and the number of ID switches is reduced to about 40%.


# Note
The above changes are for the subway pedestrian head and shoulder data set, and other scenarios can be referred to
