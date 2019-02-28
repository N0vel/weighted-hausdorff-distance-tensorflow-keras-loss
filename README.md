# Weighted Hausdorff Distance Tensorflow/Keras loss
Weighted Hausdorff Distance Loss: use it as a point cloud similarity metric based loss for keras and tf. Useful in keypoint detection.
### Attention
This loss requires a huge tensor with dimensions (number_of_pixels * number_of_keypoints if I remember correctly) of float values. So high res picture with thousands of keypoints will consume A LOT of GPU memory (at least 1 GB for 512 pixels x 512 pixels x 1000 keypoints with float32 type). 1024x1024x2000 will eat 8 GB. 
