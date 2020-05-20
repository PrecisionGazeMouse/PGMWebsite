---
title: User Manual
description: "This is meta description"
---

## System requirements

To run this software, I recommend you install a gaze tracker, such as Tobii EyeX, and a head tracker such as webcam or TrackIR. It also requires Windows 7 or higher. I’ve tested with the below hardware, but other options may work.

**Recommended Hardware:**

* [Tobii EyeX 4C](https://tobiigaming.com/products/#peripherals) (~$139)
* A webcam

**Also Supports:**

* [Tobii EyeX](https://help.tobii.com/hc/en-us/articles/212814329-What-s-the-difference-between-Tobii-Eye-Tracker-4C-and-Tobii-EyeX-) (~$79)
* [NaturalPoint TrackIR](https://www.naturalpoint.com/trackir/) (~$149)
* [NaturalPoint SmartNav](https://www.naturalpoint.com/smartnav/) (~$399)

![Precision Gaze Mouse hardware](../images/Precision%20Gaze%20Mouse%20hardware.jpg)

For head tracking my favorite option is [Enable Viacam (eViacam)](http://eviacam.crea-si.com/). It tracks your head position using a standard webcam. It's more accurate than the EyeX 4C's own head tracking, likely because it tracks many points on your face.

If you prefer infrared tracking, then TrackIR is really good. It tracks an infrared headset you clip to a hat or your headphones. It works best with contacts instead of glasses because the light from the EyeX can reflect off your glasses and distract it. It's also possible to use the SmartNav which tracks a small reflective dot.

You can use the the lower cost original EyeX, but you won’t be able to use head tracking in EyeX Only mode. Head tracking is included in version 4C of higher. The 4C is also compatible with more computers since it supports USB 2 and 3.

You also need a way to click, and there are several choices. A regular keyboard hot key can be chosen to act as a mouse click. Alternatively, you can use a USB switch. I like the Specs switch from [Ablenet]( https://www.ablenetinc.com/technology/switches/). Ablenet offers a wide variety of switches for people with different needs. Other options include the [Fragpedal](http://www.gamingmouse.com/gaming/fragpedal/dual/) to click with your foot, [Dragon](https://www.nuance.com/dragon/business-solutions/dragon-professional-individual.html) to click by speaking, or you can use dwell clicking with eViacam if you are unable to use any of these devices.

## Installation

[Install the latest release](install/publish.htm) using our installer. Next, if you have the eViacam, TrackIR or EyeX, follow the instructions below to set them up. Calibrate each and run them in the background. Lastly, start the Precision Gaze Mouse program. After initializing, the status field should say “Running”.

##### eViacam Instructions

Set your X and Y axis speeds so the mouse moves across a few inches of screen when you comfortably rotate your head. Make sure the enable eViacam hotkey is turned on and set to F11, which is the default setting. It is used to turn tracking on when using the On Key Press movement mode.

If you are using the Continuous movement mode, the feature that pauses the mouse automatically when you move it is disabled. Instead, press the pause hotkey to take over the mouse.

##### TrackIR Instructions

Choose “GazePlusMouse” in the titles tab and set it to use the One:One profile. This is the old name for the application before I renamed it. If it can't connect, it will display an error message. When you point your head directly at the center of the screen, the head position displayed should be close to (0, 0). If not, press the Center hotkey (F12 by default) in TrackIR. Also, if it says "No TrackIR connected" then verify you're running under the same user account as Precision Gaze Mouse. You may need to run TrackIR as an administrator if you also run Precision Gaze Mouse with those permissions.

If you have any trouble running the software, see the Help section below on how to file an issue.

## Settings
Here are several settings allowing you to customize the behavior of the mouse. 

![Precision Gaze Mouse Screenshot](../images/Precision%20Gaze%20Mouse%20Screenshot.png)

##### Tracker Mode

* EyeX and eViacam – Use EyeX gaze tracking to warp your mouse pointer quickly, and eViacam webcam head tracking to precisely control the pointer.
* EyeX and TrackIR – Use EyeX gaze tracking to warp your mouse pointer quickly, and TrackIR head tracking to precisely control the pointer.
* EyeX and SmartNav – Use EyeX gaze tracking to warp your mouse pointer quickly, and SmartNav head tracking to precisely control the pointer.
* EyeX Only – Use EyeX gaze tracking to warp your mouse pointer quickly, and EyeX head tracking to precisely control the pointer. Requires EyeX 4C or higher.
* TrackIR Only – Use TrackIR head tracking alone to control the mouse pointer, along with your chosen movement and click modes.
* eViacam Only – Use eViacam head tracking alone to control the mouse pointer motion, along with your chosen movement and click modes.

##### Movement

* Continuous - Will continuously follow your eye gaze as it moves around the screen.
* On Key Press - Moves the mouse when you press a hotkey, which can be less distracting for your eyes. Click the text box to change the hot key. You can also map this key to an input device, such as a USB button or switch.

##### Click On Key

An optional setting to click the mouse when you press a hotkey. It clicks on key up, so that if you use the same key for movement, you can release when the pointer is on the right spot. To double click, press twice quickly. To drag, do a double click but hold the button down on the second press. You can set the hotkey by clicking on the input box and then typing the key. Escape or Backspace will clear this setting and disable clicking.

##### Pause On Key

An optional setting to pause Precision Gaze Mouse when you press a hotkey. Normally, Precision Gaze Mouse pauses automatically when you physically move the mouse. However, when using eViacam in Continuous mode, you need to press this hot key instead. You can set the hotkey by clicking on the input box and then typing the key. Escape or Backspace will clear this setting and disable it. 

##### Sensitivity

Adjust the sensitivity for the precision mouse pointer, on a scale of 0 to 10. A setting of 0 will disable the precision mouse pointer. This is not active in eViacam mode because eViacam controls its own sensitivity.

##### Show Warp Bar

An optional setting to draw a bar below the mouse pointer. The mouse will warp to a new location when the bar turns 100% blue. 

##### Show Gaze Tracker

An optional setting to draw a grey circle indicating the warp threshold, and a grey dot where the gaze is currently looking. The mouse will warp to a new location when the dot travels outside the circle.

## Help
If you need help running or operating this mouse, please [file an issue]( https://github.com/PrecisionGazeMouse/PrecisionGazeMouse/issues) on GitHub. I’m open to suggestions and requests. 

It’s open source and I’m hoping other developers will contribute to improve it. To contribute, please see the [GitHub README](https://github.com/PrecisionGazeMouse/PrecisionGazeMouse). I’d also love to see support for this method from commercial vendors like Tobii in the future.
