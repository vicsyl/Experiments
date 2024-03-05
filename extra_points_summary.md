# Summary of experiments using extra correspondences 

* Extra correspondences are between the center of top-face (3D BB) and the midpoint of the top line segment (2D BB)   

## Modes of exploitation

### Choosing a single model from models returned by the minimal solver 

* Choosing a single model from multiple models returned by the minimal solver, based on the score with additional correspondences 
related to the minimal sample
 
* As may have been expected, this helps if #points == minimal sample, otherwise the increase in performance is usually small 
or even negative - this holds for both ARKitScenes and Metropolis datasets
* Detailed plots: 
  * [ARKitScenes](choose_single_model_arkit.md)
  * [Metropolis](choose_single_model_metropolis.md)

* Examples: ARKitScenes, <1 degree from gravity, #points == minimal sample

  * D2Px

| ![angle error levels](./data/arkit/P3P_UP2P_SP2P_verification/choose_single/mrs=UP2P/dev=1.0/DP2P_X_HOR_SIZE_RATIO/just_2/comp_arkit_verification_DP2P_X_HOR_SIZE_RATIO_general_just=p2r2_points_title_True_angle_error_levels.png) | ![position error levels](./data/arkit/P3P_UP2P_SP2P_verification/choose_single/mrs=UP2P/dev=1.0/DP2P_X_HOR_SIZE_RATIO/just_2/comp_arkit_verification_DP2P_X_HOR_SIZE_RATIO_general_just=p2r2_points_title_True_position_error_levels.png) |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

  * UP2P

| ![angle error levels](./data/arkit/P3P_UP2P_SP2P_verification/choose_single/mrs=UP2P/dev=1.0/UP2P/just_2/comp_arkit_verification_UP2P_general_just=p2r2_points_title_True_angle_error_levels.png) | ![position error levels](./data/arkit/P3P_UP2P_SP2P_verification/choose_single/mrs=UP2P/dev=1.0/UP2P/just_2/comp_arkit_verification_UP2P_general_just=p2r2_points_title_True_position_error_levels.png) |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


  * P3P

| ![angle error levels](./data/arkit/P3P_UP2P_SP2P_verification/choose_single/mrs=UP2P/dev=1.0/P3P/just_3/comp_arkit_verification_P3P_general_just=p3r3_points_title_True_angle_error_levels.png) | ![position error levels](./data/arkit/P3P_UP2P_SP2P_verification/choose_single/mrs=UP2P/dev=1.0/P3P/just_3/comp_arkit_verification_P3P_general_just=p3r3_points_title_True_position_error_levels.png) |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|



### Extra correspondences as first class citizens 

* For ARKitScenes: helps more for small deviation from gravity (the extra correspondences are not very error contaminated) than for other 
classes of camera rotation
* For ARKitScenes: helps the best for scenes with #points == minimal sample 
* For Metropolis: helps everywhere 
* Detailed plots:
  * [ARKitScenes](extra_correspondences_arkit.md)
  * [Metropolis](extra_correspondences_metropolis.md)

* Examples: Metropolis - all scenes, #points == minimal sample

  * D2Pz

| ![angle error levels](./data/metropolis/P3P_UP2P_SP2P_verification/extra_correspondence/mrs=None/DP2P_Z_HOR_SIZE_RATIO/just_2/comp_metropolis_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=p2r2_points_title_True_angle_error_levels.png) | ![position error levels](./data/metropolis/P3P_UP2P_SP2P_verification/extra_correspondence/mrs=None/DP2P_Z_HOR_SIZE_RATIO/just_2/comp_metropolis_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=p2r2_points_title_True_position_error_levels.png) |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

  * UP2P

| ![angle error levels](./data/metropolis/P3P_UP2P_SP2P_verification/extra_correspondence/mrs=None/UP2P/just_2/comp_metropolis_verification_UP2P_general_just=p2r2_points_title_True_angle_error_levels.png) | ![position error levels](./data/metropolis/P3P_UP2P_SP2P_verification/extra_correspondence/mrs=None/UP2P/just_2/comp_metropolis_verification_UP2P_general_just=p2r2_points_title_True_position_error_levels.png) |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

  * P3P

| ![angle error levels](./data/metropolis/P3P_UP2P_SP2P_verification/extra_correspondence/mrs=None/P3P/just_3/comp_metropolis_verification_P3P_general_just=p3r3_points_title_True_angle_error_levels.png) | ![position error levels](./data/metropolis/P3P_UP2P_SP2P_verification/extra_correspondence/mrs=None/P3P/just_3/comp_metropolis_verification_P3P_general_just=p3r3_points_title_True_position_error_levels.png) |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|



### All extra correspondences added to the inlier score  

* For ARKitScenes: helps quite consistently to improve performance of all solvers, mostly in the space case camera rotations
* For Metropolis: helps to improve performance for all solvers, but interestingly enough, 
it doesn't change the performance for scenes with #points == minimal sample (!!!)
* Detailed plots:
  * [ARKitScenes](inliers_all_arkit.md)
  * [Metropolis](inliers_all_metropolis.md)

* Examples: Metropolis - all scenes, #points == minimal sample

  * D2Pz

| ![angle error levels](./data/arkit/P3P_UP2P_SP2P_verification/inliers_all/mrs=UP2P/dev=1.0/DP2P_Z_HOR_SIZE_RATIO/just_2/comp_arkit_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=p2r2_points_title_True_angle_error_levels.png) | ![position error levels](./data/arkit/P3P_UP2P_SP2P_verification/inliers_all/mrs=UP2P/dev=1.0/DP2P_Z_HOR_SIZE_RATIO/just_2/comp_arkit_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=p2r2_points_title_True_position_error_levels.png) |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

  * UP2P

| ![angle error levels](./data/arkit/P3P_UP2P_SP2P_verification/inliers_all/mrs=UP2P/dev=1.0/UP2P/just_2/comp_arkit_verification_UP2P_general_just=p2r2_points_title_True_angle_error_levels.png) | ![position error levels](./data/arkit/P3P_UP2P_SP2P_verification/inliers_all/mrs=UP2P/dev=1.0/UP2P/just_2/comp_arkit_verification_UP2P_general_just=p2r2_points_title_True_position_error_levels.png) |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

  * P3P

| ![angle error levels](./data/arkit/P3P_UP2P_SP2P_verification/inliers_all/mrs=UP2P/dev=1.0/P3P/just_3/comp_arkit_verification_P3P_general_just=p3r3_points_title_True_angle_error_levels.png) | ![position error levels](./data/arkit/P3P_UP2P_SP2P_verification/inliers_all/mrs=UP2P/dev=1.0/P3P/just_3/comp_arkit_verification_P3P_general_just=p3r3_points_title_True_position_error_levels.png) |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


### Extra correspondences only related to the minimal sample are added to the inlier score

* Very similar to the previous method 
* Detailed plots:
  * [ARKitScenes](inliers_sample_arkit.md)
  * [Metropolis](inliers_sample_metropolis.md)
