# undefined > v2-trainFromV3
https://public.roboflow.ai/object-detection/undefined

Provided by undefined
License: Public Domain

## Background Information
This dataset was curated and annotated by [Mohamed Traore](https://www.linkedin.com/in/mohamed-traore-399934129/) from the [Roboflow Team](https://roboflow.com/about). A custom dataset composed of one class (chicken). The main objective is to identify chicken(s) and perform object-tracking on chicken(s) using Roboflow's "[zero shot object tracking](https://blog.roboflow.com/zero-shot-object-tracking/)."

The [original video](https://www.youtube.com/watch?v=jkt2RYpKzKk) is from *Wendy Thomas* (Description: *"Definitive proof that the chicken crossed the road to get to the other side."*)

The original custom dataset *(v1)* is composed of 106 images of chickens and their surrounding environment.

The dataset is available under the Public License.

## Zero Shot Object Tracking
* Using the video from Wendy Thomas (which was included in this dataset through the use of [Roboflow's Video Ingestion tool](https://docs.roboflow.com/adding-data/video)

![Example - Zero Shot Object Tracking](https://i.imgur.com/pWvANOg.gif)

## Getting Started
You can download this dataset for use within your own projects, or fork it into a workspace on Roboflow to create your own model.

## Dataset Versions
### Version 1 (v1) - 106 images
* **Preprocessing:** Auto-Orient
* **Augmentations:** *No augmentations applied*
* **Training Metrics:** *This version of the dataset was not trained*

### Version 2 (v2) - 106 images
* **Preprocessing:** Auto-Orient and Resize (Stretch to 416x416)
* **Augmentations:** *No augmentations applied*
* **Training Metrics:** *This version of the dataset was not trained*

### Version 3 (v3), "v1-augmented-COCO-transferLearning" - 254 images
Trained from the COCO Checkpoint in Public Models ("[transfer learning](https://blog.roboflow.com/a-primer-on-transfer-learning/)") on Roboflow
* 3x image generation

### Version 11 (v11), "v1-augmented-trainFromScratch" - 463 images
Trained [from the Version 3 training checkpoint](https://www.loom.com/share/0c909764d6794fadb759b8a58c715323).
* Modify Classes was applied to remap the "chickens" class to "rooster" (meaning "rooster" will show up for the bounding boxes when running inference).
* 3x image generation

### Version 12 (v12) - 185 images
* **Preprocessing:** Auto-Orient, Modify Classes (remap the "chickens" class to "rooster")
* **Augmentations:** *No augmentations applied*
* **Training Metrics:** *This version of the dataset was not trained*

Mohamed Traore - [LinkedIn](https://www.linkedin.com/in/mohamed-traore-399934129/)