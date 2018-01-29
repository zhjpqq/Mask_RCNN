
# 完整打印config信息

cfg=Config()

cfg.display()

-----------------------------------------

Configurations:

# 硬件信息
GPU_COUNT                      1
IMAGES_PER_GPU                 2
BATCH_SIZE                     2
STEPS_PER_EPOCH                1000
VALIDATION_STEPS               50

# 优化器超参数
LEARNING_MOMENTUM              0.9
LEARNING_RATE                  0.001
WEIGHT_DECAY                   0.0001

# 图像信息
IMAGE_MAX_DIM                  1024
IMAGE_MIN_DIM                  800
IMAGE_PADDING                  True
IMAGE_SHAPE                    [1024 1024    3]
MEAN_PIXEL                     [ 123.7  116.8  103.9]
NAME                           None
NUM_CLASSES                    1

# 骨架网络信息
BACKBONE_SHAPES                [[256 256]
 [128 128]
 [ 64  64]
 [ 32  32]
 [ 16  16]]
BACKBONE_STRIDES               [4, 8, 16, 32, 64]

# RPN信息 cls + bbox
USE_RPN_ROIS                   True
ROI_POSITIVE_RATIO             0.33
RPN_ANCHOR_RATIOS              [0.5, 1, 2]
RPN_ANCHOR_SCALES              (32, 64, 128, 256, 512)
RPN_ANCHOR_STRIDE              1
RPN_BBOX_STD_DEV               [ 0.1  0.1  0.2  0.2]
RPN_NMS_THRESHOLD              0.7
RPN_TRAIN_ANCHORS_PER_IMAGE    256


POOL_SIZE                      7
POST_NMS_ROIS_INFERENCE        1000
POST_NMS_ROIS_TRAINING         2000
TRAIN_ROIS_PER_IMAGE           200


DETECTION_MAX_INSTANCES        100
DETECTION_MIN_CONFIDENCE       0.7
DETECTION_NMS_THRESHOLD        0.3

# 掩膜信息 mask
MASK_POOL_SIZE                 14
MASK_SHAPE                     [28, 28]
MAX_GT_INSTANCES               100
MINI_MASK_SHAPE                (56, 56)
USE_MINI_MASK                  True
BBOX_STD_DEV                   [ 0.1  0.1  0.2  0.2]