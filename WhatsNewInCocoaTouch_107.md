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
* Tutorial on [Ray Wenderlich](http://www.raywenderlich.com/114552/uistackview-tutorial-introducing-stack-views)

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
* SFSafariViewController - new
  * Display webcontext but with usual Safari buttons/toolbars/functionality
  * Not simply a UIWebView replacement
    * UIWebView is just an empty frame to be contained in your view
* Safari enhancements
  * Content blocking allows blocking of certain types of content on any page rendered in Safari
  * This has serious implications for web-page based advertising
  * Potentially allows Apple more control over web advertising on iOS platform 
* Document based applications
  * See specific talk on [Building Document Based Applications](https://developer.apple.com/videos/play/wwdc2015-234/)
* New Contacts-API for interacting with contacts on the phone 
  * See separate talk on [Contacts API](https://developer.apple.com/videos/play/wwdc2015-223/)
* Wallet / Passkit enhancements
* Core Location
  * Changes in background location tracking
  * Added new one-time location request for when only occasional location tracking is needed
    * New `requestionLocation` API
* Various enhancements to:
  * HealthKit
  * HomeKit
  * CloudKit
  * GameplayKit


