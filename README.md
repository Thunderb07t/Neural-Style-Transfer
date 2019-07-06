# Neural-Style-Transfer
An image consists of 2 Parts, Content and Style. Here it is an style transfer method to transfer the style of an image to annother.
The implementation is done according to the paper: https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Gatys_Image_Style_Transfer_CVPR_2016_paper.pdf)

Here we use a pretrained VGG-19 model with all layers frozen to get the content and style layer.
Then we are required to find the relation between out style layers to extract the style from the image.
Then the style is required to be merged with content of another to create our target image.

We calculate content and style losses an then try to merge the style and content of different images while also minimising the total loss using ADAM optimizer.

Total loss is calculated as the sum of content loss and the style loss.

The final results are not the best out there, but it is a good start and can be further impproved by tuning thee hyperparameters like layer weights and using some further techniques.
