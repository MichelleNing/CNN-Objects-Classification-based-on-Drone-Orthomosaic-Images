# CNN-Objects-Classification-based-on-Drone-Orthomosaic-Images
## Land Cover Object Classification Using High Resolution Drone Imagery

Up-to-date land use and land cover information is important to many social, economic and environmental applications such as urban and regional planning, natural resources management and conservation, farming management, ecological protections and road maintanance, etc. Remotely sensed drone imagery offers a great oppotunity for extracting land cover information through the processing of image classification and interpretation at a very fine spatial scale. Traditional pixel based classification approach process the image on pixel-by-pixel basis without considering the ground object as a whole. Current development on CNN and deep learning techniques could potentially make the land cover classiftication task to be faster and more accurate. The objective of this pilot projet is to explore and test the feasibility of land cover classification using high-resolution drone data as input to my pre-designed deep learning workflow.

In our test area, five land cover types are identified: trees, buildings, crop A, crop B, and hay. Drone images (RGB) acquired over the test area are preprocessed by a third-party photogrammetry software to generate a stitched orthomosaic image. The obtained orthomosaic image is then segmented into 10m by 10m subimages. It is assumed that each subimage represents one dominant land cover class. A total of 284 subimages are selected to train, valid and test the deep learning method.

## Instruction
1. cd into the project directory

2. Download anaconda or miniconda based on the instructions in the anaconda website and miniconda website.

3. Create a new conda environment: conda create --name CNN-classification python=3

4. Enter your new environment:

Mac/Linux: >> source activate CNN-classification
Windows: >> activate CNN-classification
5. Ensure you have numpy, matplotlib, pandas, and jupyter notebook installed by doing the following: conda install numpy matplotlib pandas jupyter notebook

6. Ensure you have PyTorch, torchvision installed by doing: conda install torchvision -c pytorch
By default, GPU support is built if CUDA is found and torch.cuda.is_available() is true. It’s possible to force building GPU support by setting FORCE_CUDA=1 environment variable, which is useful when building a docker image.

Run the following to open up the notebook server: jupyter notebook
