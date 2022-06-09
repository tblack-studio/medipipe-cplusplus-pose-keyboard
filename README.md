# medipipe-cplusplus-pose-keyboard
Using mediapipe pose estimation as keyboard driver
# Run pose tracking 
    - Build: `bazel build -c opt --define MEDIAPIPE_DISABLE_GPU=1 src/pose_tracking:pose_tracking_cpu`
    
    - Webcam is ready then run: 
        ```
        GLOG_logtostderr=1 bazel-bin/src/pose_tracking/pose_tracking_cpu --calculator_graph_config_file=mediapipe/graphs/pose_tracking/pose_tracking_cpu.pbtxt
        ```
