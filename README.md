# Intention Prediction in Vehicular Environments
An undergraduate research project by Mitch Mathieu

<p align="center">
  <img src="intention_prediction.gif" alt="predicting the future positions of vehicles"/>
</p>

## Dependencies
- `python3.5+`
- `TensorFlow` (tested on 1.15)
- `opencv`
- `shapely`
- `numba`
- `easydict`
- `moviepy`

## Installation
1. Clone this repository
2. Download the 3D KITTI detection dataset from [here](http://www.cvlibs.net/datasets/kitti/eval_object.php?obj_benchmark=3d).
Files to inlcude:
    * Velodyne point clouds (29 GB): input data to VoxelNet
    * Training labels of object data set (5 MB): input label to VoxelNet
    * Camera calibration matrices of object data set (16 MB): for visualization of predictions
    * Left color images of object data set (12 GB): for visualization of predictions
    
3. Update the dataset directory in `config.py` with the new location of your data. Your dataset directory should have the following structure:
```plain
└── DATA_DIR
       ├── data_object_calib
       ├── data_object_image_2
       ├── data_object_label_2
       └── data_object_velodyne
```
4. Run the Jupyter Notebook `intention_prediction.ipynb`
