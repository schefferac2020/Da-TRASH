# Da-TRASH

In this work, our team aims to reproduce and extend upon the paper Learning RGB-D Feature Embeddings for Unseen Object Instance Segmentation by Y. Xiang et. al. This work makes use of non-photorealistic, synthetic RGB + Depth data to produce surprisingly accurate instance segmentation masks of unknown objects. In this report, our team will validate the specific result of the paper suggesting that combining RGB and depth feature vectors elementwise is most effective for this task. Additionally, our team will attempt to extend upon this work by adapting the model to produce adequate results on simple RGB images by first predicting the corresponding depth image with another machine learning model. This extension allows this instance segmentation model to be run on simpler cameras, without depth-sensing capabilities. We show improved segmentation accuracy of our new model, Da-TRASH, on trash segmentation datasets as well as traditional tabletop datasets.

Da-TRASH Architecture
![newVis](https://user-images.githubusercontent.com/29879582/233763531-27b18af0-4001-4a55-823a-820b55a046ee.png)

Da-TRASH Results Example <br>
<img width="333" alt="OSD_results" src="https://user-images.githubusercontent.com/29879582/233763529-394bc13c-1d6d-41c0-9b65-3e5a3866b00c.png">

To Run Da-TRASH on custom images, first generate depth maps using `ZoeDepth.ipynb` and then get segmentation labels using the `test_sample` function in the `OSDTesting.ipynb`

If you want to train your model use `Overfit.ipynb`
