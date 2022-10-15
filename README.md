# Handwriting Recognition IOS App
A bit of fun with IOS and Machine Learning

This IOS App is based on a [youtube video](https://www.youtube.com/watch?v=bOg8AZSFvOc) explaining all the details.
This neural network is embedded in a CoreML file, which was got from here: [http://coreml.store/mnist](http://coreml.store/mnist)
I have added later some changes to experiment a bit.

Basically, the user draws a number on the drawing area.
This picture is reduced to a 28x28 pixel format and given to a neural network, which provides a list of probabilities for each number (softmax).

I tried several things to improve the accuracy, for instance increasing the thickness of the drawing line.
I also displayed the 28x28 picture on the top left to see how the picture given to the NN was distinguishable.

Several possibilities to fix this:
- Quality might be lost when compressing to 28x28 pixels: replace the drawing pad by a 28x28 drawing area.
- The network itself might not be very effective. Find a more effective one or train it with a bigger dataset.
- I only tested on the simulator. Drawing with the mouse might give different patterns as if we drew on the phone.

