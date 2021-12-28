# Arduino Guitar Tuner

Code for arduino guitar tuner project, utilizing signal processing principles from electrical signals and systems course and integrating hardware and software. 

## Project Description

Using an [open source library](https://github.com/kosme/arduinoFFT) to perform [Fast Fourier Transforms](https://en.wikipedia.org/wiki/Fast_Fourier_transform) on the signal inputs, our algorithm would auto-identify a musical note being played from the maximum present frequency in the Fourier Transform. This would allow us to establish a target note, calculating the difference between the actual frequency and the predicted musical note. This error was calculated in the unit of cents and outputted to the user through the hardware integration of a 5 light display. Additionally, this guitar tuner has a power threshold implemented to filter out noisy input from background sounds.

### Image
<img width="278" alt="arduino" src="https://user-images.githubusercontent.com/46762539/147516054-273ac722-065c-4578-8f84-5e17740ec325.png">

## Dependencies
* [ArduinoFFT](https://github.com/kosme/arduinoFFT): Open source library to perform fast fourier transforms
