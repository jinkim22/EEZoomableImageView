# EEZoomableImageView

**Provides full screen zooming ability to UIImageView like instagram.**


![](https://media.giphy.com/media/oysCUWJjGED562VLTK/giphy.gif) 
![](https://media.giphy.com/media/2xPVtD4NxAfqj5HQpI/giphy.gif)

## What does EEZoomableImageView do?
Gives full screen zooming ability to UIImageView with no additional code.

It handles number of the touch changes on the screen. There is no weird behaviour like jumping image's center when user removes one finger from the screen, as far as I know. :squirrel:

## <br/>Setup

**Using CocoaPods (Recommended)**

Add the line below to your Podfile;

```
pod 'EEZoomableImageView'
```

Then you can install it with pod install command.

**Manual**

Download the sample project, just drag and drop the EEZoomableImageView.swift file to your project.

## <br/>Usage
Make your image view subclass of EEZoomableImageView. It's simple as that.

## <br/>Customizable Parameters
Custom parameters can be set through EEZoomableImageView instance

```
    @IBOutlet weak var zoomableImageView: EEZoomableImageView! {
        didSet {
            zoomableImageView.minZoomScale = 0.5
            zoomableImageView.maxZoomScale = 3.0
            zoomableImageView.resetAnimationDuration = 0.5
            zoomableImageView.zoomDelegate = self
        }
    }
```

* **minZoomScale:** Minimum scale of the zoom imageview. Default value is 1.00
* **maxZoomScale:** Maximum scale of the zoom imageview. Default value is 3.00
* **resetAnimationDuration:** Duration of the reset animation. Default value is 0.3 sec
* **zoomDelegate:** Zoom Delegate is informed when zooming started and ended.
* **isZoomingActive:** Flag that indicates whether zooming is active or not. (Read Only)


 ## <br/>Questions or Advices
 Just send me an email (ergunemr@gmail.com)