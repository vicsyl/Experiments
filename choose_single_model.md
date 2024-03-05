 # experiments with additional correspondences in ARKitScenes

## Adding the extra points to the potential inliers 

* Computing the inlier score with the extra points (extra points not included in the minimal samples)
* plots for #objects == #minimal-sample 


D2Px

* camera-x axis in horizontal plane < 1 degree deviation
* exactly 2 objects - 19222 imgs

| ![angle error levels](./data/P3P_UP2P_SP2P_verification/mrs=DP2Px/extra_points_ver=ia/dev=1.0/DP2P_X_HOR_SIZE_RATIO/comp_arkit_verification_DP2P_X_HOR_SIZE_RATIO_general_just=4_2_points_angle_error_levels.png) | ![position error levels](./data/P3P_UP2P_SP2P_verification/mrs=DP2Px/extra_points_ver=ia/dev=1.0/DP2P_X_HOR_SIZE_RATIO/comp_arkit_verification_DP2P_X_HOR_SIZE_RATIO_general_just=4_2_points_position_error_levels.png) |
|---|---|

* < 1 degree deviation from gravity
* exactly 2 objects - 402 imgs

| ![angle error levels](./data/P3P_UP2P_SP2P_verification/mrs=UP2P/extra_points_ver=ia/dev=1.0/DP2P_X_HOR_SIZE_RATIO/comp_arkit_verification_DP2P_X_HOR_SIZE_RATIO_general_just=4_2_points_angle_error_levels.png) | ![position error levels](./data/P3P_UP2P_SP2P_verification/mrs=UP2P/extra_points_ver=ia/dev=1.0/DP2P_X_HOR_SIZE_RATIO/comp_arkit_verification_DP2P_X_HOR_SIZE_RATIO_general_just=4_2_points_position_error_levels.png) |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

D2Pz

* camera-z axis in horizontal plane < 1 degree deviation
* exactly 2 objects - 1956 imgs

| ![angle error levels](./data/P3P_UP2P_SP2P_verification/mrs=DP2Pz/extra_points_ver=ia/dev=1.0/DP2P_Z_HOR_SIZE_RATIO/comp_arkit_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=4_2_points_angle_error_levels.png) | ![position error levels](./data/P3P_UP2P_SP2P_verification/mrs=DP2Pz/extra_points_ver=ia/dev=1.0/DP2P_Z_HOR_SIZE_RATIO/comp_arkit_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=4_2_points_position_error_levels.png) |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

* < 1 degree deviation from gravity
* exactly 2 objects - 402 imgs

| ![angle error levels](./data/P3P_UP2P_SP2P_verification/mrs=UP2P/extra_points_ver=ia/dev=1.0/DP2P_Z_HOR_SIZE_RATIO/comp_arkit_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=4_2_points_angle_error_levels.png) | ![position error levels](./data/P3P_UP2P_SP2P_verification/mrs=UP2P/extra_points_ver=ia/dev=1.0/DP2P_Z_HOR_SIZE_RATIO/comp_arkit_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=4_2_points_position_error_levels.png) |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

UP2P

* < 1 degree deviation from gravity
* exactly 2 objects - 402 imgs

| ![angle error levels](./data/P3P_UP2P_SP2P_verification/mrs=UP2P/extra_points_ver=ia/dev=1.0/UP2P/comp_arkit_verification_UP2P_general_just=4_2_points_angle_error_levels.png) | ![position error levels](./data/P3P_UP2P_SP2P_verification/mrs=UP2P/extra_points_ver=ia/dev=1.0/UP2P/comp_arkit_verification_UP2P_general_just=4_2_points_position_error_levels.png) |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

P3P

* camera-x axis in horizontal plane < 1 degree deviation
* exactly 3 objects - 6265 imgs

| ![angle error levels](./data/P3P_UP2P_SP2P_verification/mrs=DP2Px/extra_points_ver=ia/dev=1.0/P3P/comp_arkit_verification_P3P_general_just=6_3_points_angle_error_levels.png) | ![position error levels](./data/P3P_UP2P_SP2P_verification/mrs=DP2Px/extra_points_ver=ia/dev=1.0/P3P/comp_arkit_verification_P3P_general_just=6_3_points_position_error_levels.png) |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------|

the results are similar for other pose classes (camera-z axis in horizontal plane < 1 degree deviation, < 1 degree deviation from gravity) 



## Choosing a single model 

* Choosing a single model from multiple models based on the score including upper extra points
* only when #objects == #minimal-sample, plots for the same only


D2Px

* camera-x axis in horizontal plane < 1 degree deviation
* exactly 2 objects - 19222 imgs

| ![angle error levels](./data/P3P_UP2P_SP2P_verification/mrs=DP2Px/extra_points_ver=True/dev=1.0/DP2P_X_HOR_SIZE_RATIO/comp_arkit_verification_DP2P_X_HOR_SIZE_RATIO_general_just=4_2_points_angle_error_levels.png) | ![position error levels](./data/P3P_UP2P_SP2P_verification/mrs=DP2Px/extra_points_ver=True/dev=1.0/DP2P_X_HOR_SIZE_RATIO/comp_arkit_verification_DP2P_X_HOR_SIZE_RATIO_general_just=4_2_points_position_error_levels.png) |
|---|---|

* < 1 degree deviation from gravity
* exactly 2 objects - 402 imgs

| ![angle error levels](./data/P3P_UP2P_SP2P_verification/mrs=UP2P/extra_points_ver=True/dev=1.0/DP2P_X_HOR_SIZE_RATIO/comp_arkit_verification_DP2P_X_HOR_SIZE_RATIO_general_just=4_2_points_angle_error_levels.png) | ![position error levels](./data/P3P_UP2P_SP2P_verification/mrs=UP2P/extra_points_ver=True/dev=1.0/DP2P_X_HOR_SIZE_RATIO/comp_arkit_verification_DP2P_X_HOR_SIZE_RATIO_general_just=4_2_points_position_error_levels.png) |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

D2Pz

* camera-z axis in horizontal plane < 1 degree deviation
* exactly 2 objects - 1956 imgs

| ![angle error levels](./data/P3P_UP2P_SP2P_verification/mrs=DP2Pz/extra_points_ver=True/dev=1.0/DP2P_Z_HOR_SIZE_RATIO/comp_arkit_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=4_2_points_angle_error_levels.png) | ![position error levels](./data/P3P_UP2P_SP2P_verification/mrs=DP2Pz/extra_points_ver=True/dev=1.0/DP2P_Z_HOR_SIZE_RATIO/comp_arkit_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=4_2_points_position_error_levels.png) |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

* < 1 degree deviation from gravity
* exactly 2 objects - 402 imgs

| ![angle error levels](./data/P3P_UP2P_SP2P_verification/mrs=UP2P/extra_points_ver=True/dev=1.0/DP2P_Z_HOR_SIZE_RATIO/comp_arkit_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=4_2_points_angle_error_levels.png) | ![position error levels](./data/P3P_UP2P_SP2P_verification/mrs=UP2P/extra_points_ver=True/dev=1.0/DP2P_Z_HOR_SIZE_RATIO/comp_arkit_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=4_2_points_position_error_levels.png) |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

UP2P

* < 1 degree deviation from gravity
* exactly 2 objects - 402 imgs

| ![angle error levels](./data/P3P_UP2P_SP2P_verification/mrs=UP2P/extra_points_ver=True/dev=1.0/UP2P/comp_arkit_verification_UP2P_general_just=4_2_points_angle_error_levels.png) | ![position error levels](./data/P3P_UP2P_SP2P_verification/mrs=UP2P/extra_points_ver=True/dev=1.0/UP2P/comp_arkit_verification_UP2P_general_just=4_2_points_position_error_levels.png) |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

P3P

* camera-x axis in horizontal plane < 1 degree deviation
* exactly 3 objects - 6265 imgs

| ![angle error levels](./data/P3P_UP2P_SP2P_verification/mrs=DP2Px/extra_points_ver=True/dev=1.0/P3P/comp_arkit_verification_P3P_general_just=6_3_points_angle_error_levels.png) | ![position error levels](./data/P3P_UP2P_SP2P_verification/mrs=DP2Px/extra_points_ver=True/dev=1.0/P3P/comp_arkit_verification_P3P_general_just=6_3_points_position_error_levels.png) |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------|

the results are similar for other pose classes (camera-z axis in horizontal plane < 1 degree deviation, < 1 degree deviation from gravity) 

