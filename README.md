# HurricaneDamageRecognition
Submission for EY Data Science Challenge 2024

## Objective 
To develop a machine learning model to identify and detect “damaged” and “un-damaged” coastal infrastructure (residential and commercial buildings), which have been impacted by natural calamities such as hurricanes, cyclones, etc. 

## Notes
- Region: Puerto Rico
- Storm: Hurricane Maria in (2017)
- Pre Event Date - 29th Aug’17
- Post Event Date - 12th Oct’17 
- Clouds appear as saturated (dark) regions in each color band. Pre-storm image has more clouds than post storm image. 

## Challenges
- No cloud masking available, although there are clouds in the images.
- Inherent difficulty in differentiating resedential and commercial buildings.   

## Appenxdix
- __TIFF__: Tag Image File Format. Lossless form of file compression (no image quality loss).

## Technologies/Libraries Used
-LabelMe for Annotation  
-YOLOv8 deep-learning model  

## Data Annnotation Approach
Break up both pre and post hurrican images into grid. Convert grid tif to jpeg (for compatibility with LabelMe).   
Compare pre images with post while manually annotating.   
_Given that pre-images, as the name suggests, were taken prior to the Hurricane, the buildings will be undamaged. This gives the annotator a reference for identifying damaged and undamaged images, and the model could potentially be trained on pre-images for undamaged residential and commerical buildings._

## References
