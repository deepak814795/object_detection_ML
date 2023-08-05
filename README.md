# Object Detection Model Using Tensorflow and Coco SSD
## Screenshots are available at bottom of the page. <br>
This is a realtime Object detection model that aims to localize and identify multiple objects in a single image.

This model is a TensorFlow.js port of the COCO-SSD model. For more information about Tensorflow object detection API, check out this readme in tensorflow/object_detection.

This model detects objects defined in the COCO dataset, which is a large-scale object detection, segmentation, and captioning dataset. You can find more information here. The model is capable of detecting 80 classes of objects. (SSD stands for Single Shot MultiBox Detection).

It can take input as live video from webcam and returns an array of bounding boxes with class name and confidence level for the diffrent objects identified.

## API
### Loading the model
Coco-ssd is the module name, which is automatically included when you use the <script src> method. When using ES6 imports, coco-ssd is the module.<br>
Args: config Type of ModelConfig interface with following attributes:

* base: Controls the base cnn model, can be 'mobilenet_v1', 'mobilenet_v2' or 'lite_mobilenet_v2'. Defaults to 'lite_mobilenet_v2'. lite_mobilenet_v2 is smallest in size, and fastest in inference speed. mobilenet_v2 has the highest classification accuracy.

* modelUrl: An optional string that specifies custom url of the model. This is useful for area/countries that don't have access to the model hosted on GCP.

Returns a model object.
### Detecting the Objects
You can detect objects with the model without needing to create a Tensor. model.detect takes an input image element and returns an array of bounding boxes with class name and confidence level.

This method exists on the model that is loaded from cocoSsd.load.
Args:

* img: A Tensor or an image element to make a detection on. <br>
* maxNumBoxes: The maximum number of bounding boxes of detected objects. There can be multiple objects of the same class, but at different locations. Defaults to 20.
* minScore: The minimum score of the returned bounding boxes of detected objects. Value between 0 and 1. Defaults to 0.5. <br>
Returns an array of classes and probabilities that looks like:

# Screenshots of model
### Single Objects
![person](https://github.com/deepak814795/object_detection_ML/assets/91387970/af590a3c-9563-4288-84cd-78bcf8c696d3)
![cat](https://github.com/deepak814795/object_detection_ML/assets/91387970/3a845c0c-a86b-4e1b-a37b-11ca9a1e94ac)
![dog](https://github.com/deepak814795/object_detection_ML/assets/91387970/27b4cd31-73bb-4092-885e-b0376cf623bb)
![train](https://github.com/deepak814795/object_detection_ML/assets/91387970/c5f4cd49-8381-462f-9f9c-655450ecf1d7)
### Multiple Objects
![mul](https://github.com/deepak814795/object_detection_ML/assets/91387970/6137e68e-10dd-4335-8a0e-2e1e40991e66)

## Thank you for visiting!!



