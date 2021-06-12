# Augmentation-and-Annotation

## Annotation

For annotation, we made use of makesense.ai which is an open source and free to use image
annotator which intelligently annotates the images using AI.

All of the images before augmentation were annotated manually on this online software. For
annotating, a rectangle was drawn around each of the region of interest and it was labeled with a
name. 6 labels were introduced in each image as discussed above. The annotations of each image
were saved in the VOC XML format

![](https://github.com/samrafakhar/Augmentation-and-Annotation/blob/main/screenshots/1.PNG)

## Augmentation

Each XML file contains complete information about that image. This include, the folder in which the images are placed, filename, Path to image, width, height, depth, and object tags for all the labels. A sample Object tag is shown as follows

                      <object>
                              <name>Surname</name>
                              <pose>Unspecified</pose>
                              <truncated>Unspecified</truncated>
                              <difficult>Unspecified</difficult>
                              <bndbox>
                                      <xmin>148</xmin>
                                      <ymin>56</ymin>
                                      <xmax>196</xmax>
                                      <ymax>71</ymax>
                              </bndbox>
                      </object>
                      
<bndbox> block indicated the bounding box of the image. xmin, ymin represent the top left corner and xmax, ymax indicate the bottom right corner coordinates of the bounding box in the picture. <name> block is the label of the bounding box.
  
![](https://github.com/samrafakhar/Augmentation-and-Annotation/blob/main/screenshots/2.PNG)

## About the file directory
One Pakistan Passport and UK passport image is provided in the "Sample Images" folder. 
in the "Augmented Images" folder, 5 augmented images for each sample image are provided.  
The xml files in annotations folder contain the annotations for both sample images. 
The csv files contain the annotations for all augmented images generated for this project.
