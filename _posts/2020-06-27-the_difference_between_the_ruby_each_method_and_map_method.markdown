---
layout: post
title:      "The Difference Between the Ruby Each Method and Map Method"
date:       2020-06-27 05:15:28 +0000
permalink:  the_difference_between_the_ruby_each_method_and_map_method
---


### Well lets start with the Each method. 

When I first started writing ruby code I found this to be very useful, however I truly could not understand what it was doing and why ruby has different iterators.

The .each method iterates over an array, hash, or range and does not change any elements in it.

```
["1", "2", "3", "4", "5"].each do |element|
       puts element
end

#["1", "2", "3", "4", "5"]
```

Notice how this code does returns the original array.

Now what if we wanted to change something in it

```
["1", "2", "3", "4", "5"].each do |element|
       element + 1
end

#["1", "2", "3", "4", "5"]
```

Notice how this code is not changing the elements in the array all it is doing is returning the original array.

### Lets take at the Map/Collect method

The map/collect method returns a new array, its main use is to **transform** data.

```
["1", "2", "3", "4", "5"].map do |element|
       element + 1
end

#["2", "3", "4", "5", "6"]
```

Notice how .map returned a new array with the updated array elements.

In contrast the .map method will return a new array while the .each method will return the original array.





