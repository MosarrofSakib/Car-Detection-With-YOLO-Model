# Object Detection With a Pre-trained YOLO Model

This is a project I have done during the coursera 'deep learning spealization' course. This was the final project for CNN(Convolutional Neural Network) course. The pre-trained model weights, images, data and utility functions were provided by the course instructor "Andrew Ng".

On this project many of the ideas were came from two YOLO model papers: Redmon et al., 2016(https://arxiv.org/abs/1506.02640) and Redmon and Farhadi, 2016(https://arxiv.org/abs/1612.08242).

Here is an example of how the ouput will look like:
![DEMO](../master/out/test.jpg)

# Project Details

On this project we have implemented,
- Filtering with a Threshold on Class Scores (yolo_filter_boxes fuction): Filters YOLO boxes by thresholding on object and class confidence.
- YOLO Non-max Suppression (yolo_non_max_suppression function): Applies Non-max suppression (NMS) to set of boxes.
- Wrapping Up the Filtering (yolo_eval function): Converts the output of YOLO encoding (a lot of boxes) to your predicted boxes along with their scores, box coordinates and classes.
- Loading the pre-trained model weights: Loads pre-trained weights and use the model to predict the output.
- Run the YOLO on an Image (prdict function): Runs the graph to predict boxes for "image_file". Prints and plots the predictions.
