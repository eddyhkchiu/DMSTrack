<div align="center">
  
# Probabilistic 3D Multi-Object Cooperative Tracking for Autonomous Driving via Differentiable Multi-Sensor Kalman Filter

Hsu-kuang Chiu<sup>1</sup>, Chien-Yi Wang<sup>2</sup>, Min-Hung Chen<sup>2</sup>, Stephen F. Smith<sup>1</sup>

<sup>1</sup>Robotics Institute, Carnegie Mellon University, <sup>2</sup>NVIDIA Research

[arxiv](https://arxiv.org/abs/2309.14655)

<img src="images/project_page_fig1.jpg" height=400px>

</div>

## Overview

We propose a novel algorithm: Differentiable Multi-Sensor Kalman Filter for 3D Multi-Object Cooperative Tracking (DMSTrack). Our algorithm is designed to be capable of estimating observation noise covariance of each detection from different Connected Autonomous Vehicles (CAVs) to better take advantage of the Kalman Filter’s theoretical optimality property: minimizing the expected error of state estimation. 

To train our Differentiable Multi-Sensor Kalman Filter neural model, we use each detection's local point cloud BEV feature and the positional feature as input. We calculate the regression loss by measureing the difference between the tracking result and the ground-truth. For more details, please refer to our paper at [arxiv](https://arxiv.org/abs/2309.14655).

The experiment results show that our algorithm improves the tracking accuracy by 17% with only 0.037x communication costs compared with the state-of-the-art method in V2V4Real\[1].
  
