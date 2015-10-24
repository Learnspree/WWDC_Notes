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
    * Note: External labels don't apply to first parameter in a method as that is implied by convention in the method name (e.g. '''displayMapForCountry(country: String)'''). This is similar to Obective-C convention.

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


