# Scanbot SDK Example Apps for Android

These example apps show how to integrate the [Scanbot SDK](https://scanbot.io/sdk.html) for Android.


## What is Scanbot SDK?

The Scanbot SDK brings scanning and document creation capabilities to your mobile apps.
It contains modules which are individually licensable as license packages.
For more details visit our website https://scanbot.io/sdk.html


## Documentation

To get started please check out our Wiki: https://github.com/doo/Scanbot-SDK-Examples/wiki

JavaDocs of the Scanbot SDK for Android can be found here: http://doo.github.io/Scanbot-SDK-Documentation/Android/


## License key

You can run our examples and even develop your app without a license key.
If you do not specify a license key in the `AndroidManifest.xml` file then the SDK will work in **trial mode (trial period of 1 minute)**.
After the trial period is over the Scanbot SDK functions will stop working. UI components (like CameraView) will freeze or may be terminated.
You can just restart the app to get another trial period.

If you require a free trial license which works for a longer period of time please contact us at sdk@scanbot.io.

Please note: The SDK with a trial license should only be used for evaluation and testing purposes or during the development phase.
A trial license is not developed to be integrated into your production apps!


## Pitfalls & issues

Please see https://github.com/doo/Scanbot-SDK-Examples/wiki/Pitfalls-%26-issues


## What is the latest version of the SDK?

The current version of the Scanbot SDK for Android is **1.25.0**


## Changelog of the Scanbot SDK for Android

##### 1.25.0
* Added Barcode/QR code scanner feature to the Scanbot SDK package 1

##### 1.24.0
* Optimized transitive dependencies for Scanbot SDK library
* Stop supporting `armeabi` architecture

##### 1.23.3
* Fixed contour detection and autosnapping freeze on the autofocus tap

##### 1.23.2
* Added `detectionScore` value in `DetectedFrame` class
* Fixed 180 degree camera preview rotation

##### 1.23.0
* Added Scanbot SDK package 3 with SEPA Pay Form scanner feature

##### 1.22.6
* Fixed bug when `ScanbotCameraView` crashes with `IllegalStateException` after `onPause`

##### 1.22.5
* Added methods for setting contour detector parameters in `ContourDetectorFrameHandler`

##### 1.22.4
* Added methods for setting OCR and language classifier blobs paths in `ScanbotSDKInitializer`
* Updated version of transitive dependencies

##### 1.22.3
* Added continuous focus option for `ScanbotCameraView`

##### 1.22.2
* Added method that provides internal OCR blobs directory in `BlobManager` in SDK-2

##### 1.22.1
* Added methods for performing OCR with multiple predefined languages in `TextRecognition` in SDK-2

##### 1.22.0
* Scanbot SDK was switched from RoboGuice DI to Dagger 2

##### 1.21.3
* Fixed minor camera issues
* Added setters for edge width and color in `EditPolygonImageView`

##### 1.21.2
* Fixed dependencies in SDK packages

##### 1.21.1
* Added camera preview and picture size setters in `ScanbotCameraView`
* Added camera orientation locks in `ScanbotCameraView`

##### 1.19.0
* Fixed issue when `EditPolygonImageView` with `MagnifierView` was working only as part of an `Activity`.
* Removed `DrawMagnifierListener`.

##### 1.18.4
* `EditPolygonImageView` was not working properly on Android Nougat.

##### 1.18.2
* It was not possible to create PDFs without embedded text in SDK-2

##### 1.18.1
* Fixed crash related to text recognition

##### 1.18.0
* It's now possible to perform OCR without sandwiched PDF as part of result

##### 1.17.0
* It's now possible to customize the `Logger` implementation used by the SDK.

##### 1.16.0
* Added `ContourDetector.processImageAndRelease` - more memory efficient version of `ContourDetector.processImageF`.

##### 1.15.3
* Fixed build issues of OCR example.

##### 1.15.1
* Removed uses-feature android.hardware.camera. Camera is now optional.

##### 1.14.0
* Removed unused dependencies. Removed permission declarations from Package 1. Users are now responsible for declaring permissions. For more information see [this page](https://github.com/doo/Scanbot-SDK-Examples/wiki/Permissions).

##### 1.13.1
* Fixed bug when final image contained less than preview image from camera stream.

##### 1.13.0
* Added `ImageQualityOptimizer` which allows you to optimize image size.

##### 1.12.2
* Fixed bug when `AutosnappingController` stop operating after `onPause`.

##### 1.12.1
* Color-document filter was disabled in `ContourDetector`. Now it works again.

##### 1.12.0
* Added `ScanbotSDKInitializer#withLogging()` method which allows you to turn on logging for SDK (disabled by default).
* Improved edge detection.
* Added new filter to `ContourDetector`.

##### 1.11.0
* Added `ScanbotSDK.isLicenseActive()` method.
