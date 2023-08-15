# Object Detection Model Using Tensorflow and Coco SSD
### Site is live at https://64b75cc1af2fd3406c9d2378--capable-griffin-404c4a.netlify.app/
## Screenshots are available at bottom of the page. <br>
This is a realtime Object detection model that aims to localize and identify multiple objects in a single image.
## Tech Stack Used->
#### Tensorflow.Js : Tensorflow is an end-to-end open source platform for machine learning. It has a comprehensive, flexible ecosystem of tools, libraries, and community resources. It provides stable Python and C++ APIs, as well as a non-guaranteed backward compatible API for other languages.
#### Coco SSD model : COCO is a large-scale object detection, segmentation, and captioning dataset. It contains 80 classes of obkects.
#### React.JS : ReactJS is a declarative, efficient, and flexible JavaScript library for building user interfaces. It is an open-source, component-based front-end library that is responsible only for the view layer of the application.

## API
### Loading the model
Coco-ssd is the module name, which is automatically included when you use the <script src> method. When using ES6 imports, coco-ssd is the module.<br>
Args: config Type of ModelConfig interface with following attributes:
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



