## Resources

As expected, the reconstruction is the best from the largest model:

![](./rd_estimation/resources/recontruction_DA3NESTED-GIANT-LARGE-1.1_5.png)

notice the edge of the building on the left - it is a bit bounded. For comparison, the reconstuction is the much better than from the smallest model - here: 

![](./rd_estimation/resources/recontruction_SMALL_5.png)

These reconstructions are from just 5 images. If I add all images from the dataset (62 images from the distorted camera), there will appear some artifacts: 

![](./rd_estimation/resources/recontruction_DA3NESTED-GIANT-LARGE-1.1_ALL.png)

The visualizations of the rays do not reveal much, although it can be seen that the rays on the right do not align with the wall of the building

![](./rd_estimation/resources/recontruction_DA3NESTED-GIANT-LARGE-1.1_5_rays_cam0.png)



