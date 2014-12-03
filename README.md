SwiftlyLRU
==========

A simple and easy to use Least Recently Used "LRU" Cache written in Swift. SwiftlyLRU is implemented using a LinkedList and Swift Dictionary collection type.

```swift
//
// Example
//

import Foundation

//...

var cache = SwiftlyLRU<String, Float>(capacity: 7)

    cache["AAPL"] = 114.63
    cache["GOOG"] = 533.75
    cache["YHOO"] = 50.67
    cache["TWTR"] = 38.91
    cache["BABA"] = 109.89
    cache["YELP"] = 55.17
    cache["BABA"] = 109.80
    cache["TSLA"] = 231.43
    cache["AAPL"] = 113.41
    cache["GOOG"] = 533.60
    cache["AAPL"] = 113.01
    
    println(cache)

/*
    SwiftlyLRU Cache(7) 
    Key: AAPL Value: Optional(113.01) 
    Key: GOOG Value: Optional(533.6) 
    Key: TSLA Value: Optional(231.43) 
    Key: BABA Value: Optional(109.8) 
    Key: YELP Value: Optional(55.17) 
    Key: TWTR Value: Optional(38.91) 
    Key: YHOO Value: Optional(50.67) 
*/

//...
```
##Instillation:
Simply drag SwiftlyLRU.swift file from the Source folder into your target project.

##Reference Notes:

##Performance:
Time: O(1), Space: O(1) assumes no collisions into the hashtable.
