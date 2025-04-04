# Virtual Glasses Try on

Implementation of virtual glasses using Three.js + TensorFlow.js + Facemesh model. 

Experience the cutting-edge fusion of computer vision and augmented reality

Allowing users to try on various 3D glasses in real-time.

## Installing
Install three.js
``` bash
npm install --save three
```
Point your localhost to the cloned root directory

Browse to http://localhost/index.html 

## Face Keypoints 
The facemesh detected keypoints that used for overlay the 3D Glasses:
* Middle between Eyes : 168
* Left Eye : 143
* Bottom of Nose : 2
* Right Eye : 372

## Try glasses on
* Click "Try it On" to turn on the Webcam switch, and allowing the browser to access your webcam 
* Wait for a few seconds to Load Model for face landmark detection
* Choose the 3d glasses you would like to try on, watch yourself in fashion

## Notes
* Please note that on IOS Safari, cameras can only be accessed via the https protocol 
* Facemesh model is designed for front-facing cameras on mobile devices, where faces in view tend to occupy a relatively large fraction of the canvas. MediaPipe Facemesh may struggle to identify far-away faces.

## Library
* [jquery](https://code.jquery.com/jquery-3.3.1.min.js) - JQuery
* [three.js](https://threejs.org/) - JavaScript 3D Library
* [webcam-easy.js](https://github.com/bensonruan/webcam-easy) - javascript library for accessing webcam stream and taking photos
* [facemesh](https://github.com/tensorflow/tfjs-models/tree/master/facemesh) - MediaPipe Facemesh is a lightweight machine learning pipeline predicting 486 3D facial landmarks to infer the approximate surface geometry of a human face

