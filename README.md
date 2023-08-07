# Super-Resolution Using ESPCN Model

This project focuses on super-resolution using the Enhanced Super-Resolution Convolutional Network (ESPCN) model. The goal is to upscale low-resolution images to high-resolution images using the CelebA dataset, which contains high-resolution celebrity face images. The ESPCN model is designed specifically for single-image super-resolution tasks and leverages Convolutional layers along with the Depth-to-Space layer for upscaling.

## Dataset

The dataset used in this project is the CelebA dataset, consisting of high-resolution celebrity face images. The images are processed during data preprocessing to normalize pixel values and extract the Y channel from RGB images for training. The Y channel is then resized to a low-resolution input size of 32x32.

## Model Architecture

The ESPCN model comprises several Convolutional layers  to extract essential features from the input images. The last Convolutional layer has filters corresponding to several times the upscale factor squared, which determines the upscaling ratio. The Depth-to-Space layer is responsible for upscaling the low-resolution input to high-resolution output, achieving super-resolution.

## Training and Evaluation

For training, we use the Adam optimizer with Mean Squared Error (MSE) loss to train the ESPCN model. During training, we evaluate the model's performance using Peak Signal-to-Noise Ratio (PSNR) scores and loss curves. These metrics help monitor the model's progress in upscaling the low-resolution images to high-resolution.

## Results and Visualizations

The project presents the key findings and outcomes from the experiment. We visualize the low-resolution input images alongside their corresponding predicted high-resolution output images. This allows us to assess the effectiveness of the ESPCN model in enhancing image quality through super-resolution.

## Conclusion and Future Directions

In conclusion, the ESPCN model shows promising results in upscaling low-resolution images to high-resolution using the CelebA dataset. The project explores potential applications of the model in image restoration and facial recognition.

Future directions for this project may involve exploring different model architectures, incorporating advanced data augmentation techniques, or evaluating the model on other datasets.


