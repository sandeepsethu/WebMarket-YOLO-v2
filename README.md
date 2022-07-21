# WebMarket-YOLO-v2

The WebMarket Dataset was obtained from  https://www.kaggle.com/datasets/manikchitralwar/webmarket-dataset.


This included the dataset of images as well as a csv file with the bounding boxes for the images.

First, the bounding boxes csv was used to create txt files for the annotations/labels for the images. This was done using the script available here:  https://github.com/sandeepsethu/WebMarket-YOLO-v2/blob/main/create_labels_as_text_files.ipynb


This included cleaning the data and modifying it to the YOLO format of x_center, y_center, width and height.

After this, the dataset was split into train, test and validation split. This was done using the script at: https://github.com/sandeepsethu/WebMarket-YOLO-v2/blob/main/create_train%2Ctest%2Cval_split.ipynb

The dataset obtained after this with the whole directory was uploaded to github @ https://github.com/sandeepsethu/WebMarket-YOLO-v2/tree/main/dataset

The https://github.com/sandeepsethu/WebMarket-YOLO-v2/blob/main/yolov3x.yaml and https://github.com/sandeepsethu/WebMarket-YOLO-v2/blob/main/webmarket.yaml are the configuration files for the model which were modified for just one class and uploaded to google drive as well.

The dataset and the config files were then used along with the YOLOv3 model available at: https://github.com/ultralytics/yolov3 in the script https://github.com/sandeepsethu/WebMarket-YOLO-v2/blob/main/WEBMARKET_YOLO(1).ipynb to train YOLO on the dataset.

Best weights obtained were downloaded and uploaded to google drive as mentioned here : https://github.com/sandeepsethu/WebMarket-YOLO-v2/blob/main/best-weights.readme

The script also includes the final inference and visualizations of the confidence scores.


<iframe src="https://wandb.ai/sandeepsethu/YOLOv3/reports/Training-Report--VmlldzoyMzU1NDY0" style="border:none;height:1024px;width:100%">
