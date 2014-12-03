SwiftlyLRU
==========

```swift
//
// Example
//

import Foundation

//...

//Create cache with capacity
var cache = SwiftlyLRU<String, Float>(capacity: 7)

    //Add Key, Value pairs
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
    
    //Describe
    println(cache)

/* OUTPUT
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
SwiftlyLRU uses generics and can store any value including nil as the value and keys that confirm to the Hashable protocol. Swift’s basic types (such as String, Int, Double, Float, and Bool) are hashable by default.

##Performance:
Time: O(1), Space: O(1) assumes no collisions into the hashtable.

##Legal:
//
// Copyright (c) 2014 Justin M Fischer
//
// Permission is hereby granted, free of charge, to any person obtaining a copy of
// this software and associated documentation files (the "Software"), to deal in
// the Software without restriction, including without limitation the rights to
// use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
// the Software, and to permit persons to whom the Software is furnished to do so,
// subject to the following conditions:
//
// The above copyright notice and this permission notice shall be included in all
// copies or substantial portions of the Software.
//
// THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
// IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
// FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
// COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
// IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
// CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
//
//  Created by JUSTIN M FISCHER on 12/1/14.
//  Copyright (c) 2013 Justin M Fischer. All rights reserved.
//
