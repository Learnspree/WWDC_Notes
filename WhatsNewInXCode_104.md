# Whats new in XCode (Session 104)

## New in Swift:
* Error handling
* Protocol Extensions
* Availability (API for checking OS support for different API functions)
* Testability (test bundles can view internal API - broader test coverage without exposing private functionality)
* XCode 7 migrator helps this process (XTRAC used this)

## New in Obective-C:
* Generics
* Nullability annotations (handy for interaction with optionals in swift)

## New in XCode:
* Playgrounds improvements (rich comments etc)
* Watch OS 2 support
* StackView
* iPad multitasking (via size classes)
* App thinning
  * BitCode (intermediate layer to allow App Store to optimize)
    * turned on by default
  * Slicing
    * only include images for the calling device (e.g. 3x)
    * Using asset-catalogs will enable this automatically
    * Includes data assets / custom assets not just images and can be based on memory swell as resolution of device
  * On Demand resources 
    * for games: download next level when needed only
    * use asset tagging to allow on-demand resource downloads
    * see new resource-tags section in project overview in Xcode
    * see 15:00 for working example in video
  * Debugging
    * Added energy-impact debugger tool (in addition to CPU usage etc)
    * Address-sanitizer (Xcode will monitor memory usage in c/objective-c code to pre-empt intermittent errors accessing deallocated memory etc)
    * crash logs through organzier window via test-flight / app-store submitted apps
      * see 27:00 in video
      * debug code automatically from each crash in Xcode complete with stack trace etc
  * Testing
    * XCode Server automatically runs unit tests via test bots (previously available)
    * UI Testing is new (see 33:00 for demo)
      * record/play features
      * automatcailly generate code in test via record feature
      * add your own assertions
      * works well with Xcode server for automated testing
    * Added code coverage data (see 32:00 in video)

## Watch OS 2:
* Watchkit complications
* Native watch extensions
  * app and app extension both run natively on the watch
  * xcode 7 has automatic upgrader (“update to recommended settings”)
    * configured watch targets
    * configured extension to be copied inside the watch app so it’s installed together

