## The reconstruction

As expected, the [reconstruction](rd_estimation/resources/reconstruction_largest_5_images.glb) is the best from the largest model:

![](./rd_estimation/resources/recontruction_DA3NESTED-GIANT-LARGE-1.1_5.png)

notice the edge of the building on the left - it is a bit bounded. For comparison, this is much better than the [reconstruction](rd_estimation/resources/reconstruction_smallest_5_images.glb) from the smallest model - here: 

![](./rd_estimation/resources/recontruction_SMALL_5.png)

These reconstructions are from just 5 images. If I add all images from the dataset (62 images from the distorted camera), there will appear some artifacts in the [reconstruction](rd_estimation/resources/reconstruction_largest_all_images.glb): 

![](./rd_estimation/resources/recontruction_DA3NESTED-GIANT-LARGE-1.1_ALL.png)

The [visualization](rd_estimation/resources/reconstruction_larges_5_images_rays_img_0.glb) of the rays do not reveal much, although it can be seen that the rays on the right do not align with the wall of the building

![](./rd_estimation/resources/recontruction_DA3NESTED-GIANT-LARGE-1.1_5_rays_cam0.png)


## The correspondences

This shows correspondences between the intersections (3D) of the rays and the image plane and the 2D coordinates of the grid of the image. Indeed for this image the radial distortion is estimated fairly correctly (-0.9 vs GT=-0.81).    

![](./rd_estimation/resources/correspondences_LARGE_5_img_0.png)


## Results

These plots show the ratio between the estimated and the GT radial distortion parameter for all the distorted images in the 'rotunda' dataset. The values are clamped at the maximum of 10. The results for the largest (top) and the smallest (bottom) model are quite similar. They are somewhat odd, but still lean to the GT value. 


![](./rd_estimation/resources/rd_over_gt_rd__model=DA3NESTED-GIANT-LARGE-1.1__image_limit=None.png)

![](./rd_estimation/resources/rd_over_gt_rd__model=DA3-SMALL__image_limit=None.png)


However, the focal length estimation overestimates f quite much. These plots show the ratio between the estimated and the GT f for all the distorted images in the 'rotunda' dataset. The values are clamped at the maximum of 10. The results for the largest (top) and the smallest (bottom) model are quite similar.

![](./rd_estimation/resources/f_over_gt_f__model=DA3NESTED-GIANT-LARGE-1.1__image_limit=None.png)

![](./rd_estimation/resources/f_over_gt_f__model=DA3-SMALL__image_limit=None.png)



