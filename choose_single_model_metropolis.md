# Choosing a single model in the Metropolis dataset

* Experiments comparing baseline with version choosing a single model from multiple models returned by the minimal solver,
based on the score with additional correspondences  
 
* As may have been expected, this helps if #points == minimal sample, otherwise the increase in performance is usually small 
or even negative    

* DP2P improved more than UP2P 


## All scenes

### D2Pz

| ![angle error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/DP2P_Z_HOR_SIZE_RATIO/all/comp_metropolis_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=_points_title_True_angle_error_levels.png) | ![position error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/DP2P_Z_HOR_SIZE_RATIO/all/comp_metropolis_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=_points_title_True_position_error_levels.png) |
|---|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


| ![angle error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/DP2P_Z_HOR_SIZE_RATIO/just_2/comp_metropolis_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=p2r2_points_title_True_angle_error_levels.png) | ![position error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/DP2P_Z_HOR_SIZE_RATIO/just_2/comp_metropolis_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=p2r2_points_title_True_position_error_levels.png) |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


| ![angle error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/DP2P_Z_HOR_SIZE_RATIO/min_points=3/comp_metropolis_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=p3_points_title_True_angle_error_levels.png) | ![position error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/DP2P_Z_HOR_SIZE_RATIO/min_points=3/comp_metropolis_verification_DP2P_Z_HOR_SIZE_RATIO_general_just=p3_points_title_True_position_error_levels.png) |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

### UP2P

| ![angle error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/UP2P/all/comp_metropolis_verification_UP2P_general_just=_points_title_True_angle_error_levels.png) | ![position error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/UP2P/all/comp_metropolis_verification_UP2P_general_just=_points_title_True_position_error_levels.png) |
|---|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


| ![angle error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/UP2P/just_2/comp_metropolis_verification_UP2P_general_just=p2r2_points_title_True_angle_error_levels.png) | ![position error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/UP2P/just_2/comp_metropolis_verification_UP2P_general_just=p2r2_points_title_True_position_error_levels.png) |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


| ![angle error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/UP2P/min_points=3/comp_metropolis_verification_UP2P_general_just=p3_points_title_True_angle_error_levels.png) | ![position error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/UP2P/min_points=3/comp_metropolis_verification_UP2P_general_just=p3_points_title_True_position_error_levels.png) |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

### P3P

| ![angle error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/P3P/all/comp_metropolis_verification_P3P_general_just=_points_title_True_angle_error_levels.png) | ![position error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/P3P/all/comp_metropolis_verification_P3P_general_just=_points_title_True_position_error_levels.png) |
|---|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


| ![angle error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/P3P/just_3/comp_metropolis_verification_P3P_general_just=p3r3_points_title_True_angle_error_levels.png) | ![position error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/P3P/just_3/comp_metropolis_verification_P3P_general_just=p3r3_points_title_True_position_error_levels.png) |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


| ![angle error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/P3P/min_points=4/comp_metropolis_verification_P3P_general_just=p4_points_title_True_angle_error_levels.png) | ![position error levels](./data/metropolis/P3P_UP2P_SP2P_verification/choose_single/mrs=None/P3P/min_points=4/comp_metropolis_verification_P3P_general_just=p4_points_title_True_position_error_levels.png) |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

