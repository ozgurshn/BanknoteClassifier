# Resnet50 with CoreML

This is the **Resnet50** neural network running on the shiny new CoreML framework. It uses fine-tuned Resnet50 to recognize Turkish banknotes.

It runs from a live video feed and performs a prediction as often as it can manage. If your device becomes too hot, change the `setUpCamera()` method in **ViewController.swift** to do `videoCapture.fps = 5`.

![Alt Text](https://github.com/ozgurshn/BanknoteClassifier/blob/master/MLApp.gif)

NOTE: The reported "elapsed" time is how long it takes the Resnet50 neural net to process a single image. The FPS is the actual throughput achieved by the app.

Forked from https://github.com/hollance/Inception-CoreML
