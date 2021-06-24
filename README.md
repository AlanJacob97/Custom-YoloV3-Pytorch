# Modified-YOLO-with-custom-Dataset

Custom Dataset Construction

We trained our model on both the COCO and Open Images dataset. We did this by extracting images and there respective annotations to build a custom dataset.

Steps for coco :
Copy the file paths for annoations and images folder and paste it in extract.py. Run it to get the custom dataset in yolo format.

Steps for open images dataset :
1. Install the Oid toolkit
2. Oid toolkit will help extract specific classes and their labels
3. After obtaining the images and annotations, we must convert them to the required yolo format by running extracting_and_converting_annotations.py
4. We next generate train.txt and test.txt. For this we copy the path of images in creating-train-test-txt-files.py
5.  Also for the yolo format we create .names and .data files by pasting the image folder path in creating-files-data-and-names.py

After this copy .data .names in config folder

Instruction for running train_oid.py

1. After following the steps we include all the paths of image,.names,.data,.wts in train_oid.py
3. Run train_oid.py

Refer the presentation and the video to view the results 
References:
https://github.com/EscVM/OIDv4_ToolKit.git
https://github.com/AlphaArslan/ML_COCO_extract_specific_classes
https://www.udemy.com/course/training-yolo-v3-for-objects-detection-with-custom-data/learn/lecture/
https://towardsdatascience.com/training-yolo-for-object-detection-in-pytorch-with-your-custom-dataset-the-simple-way-1aa6f56cf7d9
https://towardsdatascience.com/object-detection-and-tracking-in-pytorch-b3cf1a696a98
https://github.com/cfotache/pytorch_custom_yolo_training