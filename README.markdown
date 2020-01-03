# Resnet50 with CoreML


[Yapay Zeka Destekli Görüntü Tanıyan iOS Uygulama Nasıl Geliştirilir?](https://medium.com/@ozgurs/g%C3%B6r%C3%BCnt%C3%BC-tan%C4%B1yan-mobil-uygulama-nas%C4%B1l-geli%C5%9Ftirilir-33760f7d827?)

[How to fine-tune ResNet in Keras and use it in an iOS App via Core ML](https://heartbeat.fritz.ai/how-to-fine-tune-resnet-in-keras-and-use-it-in-an-ios-app-via-core-ml-ee7fd84c1b26)

This is the **Resnet50** neural network running on the CoreML framework. It uses fine-tuned Resnet50 to recognize Turkish banknotes.

It runs from a live video feed and performs a prediction as often as it can manage. If your device becomes too hot, change the `setUpCamera()` method in **ViewController.swift** to do `videoCapture.fps = 5`.

![Alt Text](https://github.com/ozgurshn/BanknoteClassifier/blob/master/MLApp.gif)

NOTE: The reported "elapsed" time is how long it takes the Resnet50 neural net to process a single image. The FPS is the actual throughput achieved by the app.

Forked from https://github.com/hollance/Inception-CoreML
