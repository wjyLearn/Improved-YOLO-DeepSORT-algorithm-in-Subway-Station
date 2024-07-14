We optimized and combined the YOLOv8 detection model and DeepSORT tracking algorithm, and applied it to the passenger flow statistics of subway stations to achieve real-time statistics of passenger flow count, speed and density at key locations. The passenger flow information obtained can help the management department to adjust the operation strategy in time, ensure the safety of the station and improve the operation efficiency.


# Yolov8
Based on the improvement of YOLOv8 network, the output module with high dimensional features is removed in Head layer to simplify the model. A new fusion module is added in the Neck layer to fully integrate the feature information of different scales. CBAM attention mechanism is added to Backbone layer to enhance the extraction of useful feature information.

