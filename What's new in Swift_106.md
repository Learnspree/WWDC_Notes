# Whats new in Swift (Session 106)

## Swift 1.2:
* Not covered in this video - this concentrates on Swift 2.0
* For 1.2 see the XCode-6 release notes / fundamentals

## Enums:
* Associated values using generics
* Print to string by default now supported without assigning a string value
* Recursive enum constructs supported
* Support for grouping option types (todo: get example)

## Language / Keywords:
* 'repeat' keyword replaces 'do...while'
  * 'do' keyword now used in error handling (see later)
* Standardization of paramter labels across global and class methods
  * use of '_' to remove the requirement of a caller to use the external label
    * Note: External label defaults to internal label if none is specified in the method signature
    * Note: External labels don't apply to first parameter in a method as that is implied by convention in the method name (e.g. 'displayMapForCountry(country: String)'). This is similar to Obective-C convention.
* `if let` construct
  * the `if let` construct was improved in Swift 1.2 to allow multiple `if let` assignments/checks in the same statement
  * more improvements in Swift 2.0
    * early exits that followed the "`if/let/return`" pattern used to make code hard to read and result in multiple code paths - complicating maintenance and increasing potentially the number of unit tests you need to write
    * new "`guard`" statement introduced which allows checking for all of these "return" conditions at start of method in a single block
    * This allows the use of any optional variables after the guard statement without even the need to force-unwrap with a "`!`" operator
    * See 17:00 in the [WWDC Video](https://developer.apple.com/videos/play/wwdc2015-106/)
* new pattern matching in `if` statements
  * rather than verbose `switch` statements with multiple `case` statements, we can now use the `case` pattern matching directly in an `if` statement. 
  * See 18:35 in 
  * More details at [Natasha the Robot's Blog](http://natashatherobot.com/swift-2-pattern-matching-with-if-case/)

## Availability Checking
* Previous versions of swift required the old Objective-C style checking for a specific available selector on a class. For example, 'if (myCocoaClass.respondsToSelector(Selector("myCocoaMethod")))'
* Now you don't need to do any checking in some cases. The compiler will do all checks against your minimum supported iOS version and flag any methods used that don't comply with that.
* Also, for specific checking of a method you can use new syntax: 
     '''
     if #available(iOS 9, *) {
       // use UIStackView
     } else {
       // show sad face emoji
     }
     '''
* See [Hacking with Swift Blog](https://www.hackingwithswift.com/new-syntax-swift-2-availability-checking)

## Compiler:
* Better errors and warnings at compile time

## Testing: 
* Code is built by default in a mode where both public and private methods are accessible to unit-tests. 
* See 14:00 in [WWDC Video](https://developer.apple.com/videos/play/wwdc2015-106/)
* Use @testable attribute on any import statement in the test class 
* More details in the Unit Testing talk (link TODO)

## Documentation:
* Rich Comments - Automatic rich document generation via structured comments 
* See 14:30 [WWDC Video](https://developer.apple.com/videos/play/wwdc2015-106/)


