# Raccoon Detector
This project follows the instruction at (http://www.dat-tran.com/) and (https://www.youtube.com/watch?v=COlbP62-B-U&list=PLQVvvaa0QuDcNK5GeCQnxYnSSaar2tpku).

This dataset is coppied from DatTran's repo (https://github.com/datitran/raccoon_dataset), then I trained it from scratch and update trained model to 'output_raccon_graph' folder. Images are from Google and Pixabay. In total, there are 200 images (160 are used for training and 40 for validation).

The [TensorFlow's Object Detection API] can be downloaded from (https://github.com/tensorflow/models/tree/master/research/object_detection). 

##### Folder Structure:
```
+ annotations: contains the xml files in PASCAL VOC format
+ data: contains the input file for the TF object detection API and the label files (csv)
+ images: contains the image data in jpg format
+ training: contains the pipeline configuration file, checkpoints and labelmap
  - a few handy scripts: generate_tfrecord.py is used to generate the input files
                          for the TF API and xml_to_csv.py is used to convert the xml files into one csv
  - a few jupyter notebooks: draw boxes is used to plot some of the data and
                              split labels is used to split the full labels into train and test labels
+ output_raccon_graph: contains frozen model
```

