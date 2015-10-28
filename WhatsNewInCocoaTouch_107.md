# What's New In Cocoa Touch (Session 107)

## Size Classes in Layout
* Auto-Layout was added in iOS 6
* Adaptivity via Size Classes was added iOS 8 and lays the foundation for multi-tasking
* Layouts are no longer about "which device am I running on" 
* Now same device needs automatically different layouts when multitasking is engaged or modified
* PiP (Picture-in-Picture) is also added
* Multiple other WWDC 2015 talks on multitasking

## UIStackView
* Much easier now to do complex layouts without having to deal with many overlapping constraints
* Horizontal or Vertical stack views
* Stack View allows nesting of multiple stack views within
* A layout feature that's been in Android for some time and now finally in iOS
* Recommended for use going forward as much as possible
* Note: Early adoption will be difficult as it requires a minimum deployment target of iOS 9.0. Only for apps supporting that version of iOS and higher.

## Other UI Enhancements
* Customizable Keyboard Shortcut Bar
  * New classes added to allow developers to create individual keyboard customization buttons in the keyboard shortcut bar
  * See 8:00 at [WWDC Video](https://developer.apple.com/videos/play/wwdc2015-107/)
* Right-to-left view support for right-to-left languages/cultures
* Various UIKit enhancements including for animations
* Touch Events 
  * Up to now there is an inherent and unavoidable certain latency in touch actions by the user and the event being triggered
  * Apple claim this is industry leading latency even before iOS 9
  * New events will be fired in iOS 9 which use a complex new engine to "predict" the upcoming events based on the users' gestures
  * A good example of this features at about 15:10 in the [WWDC Video](https://developer.apple.com/videos/play/wwdc2015-107/)
* Notifications now accept text input
  * For example allow responding to text message directly within the notification


