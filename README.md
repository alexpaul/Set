# Set

## Initializing a Set
```swift 
// initializing a Set
var babyName: Set<String> = ["Kim", "Hua", "Bertie", "Esther"]
var cohorts: Set = [1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0]
```

## Combining Sets

#### `update(with:_)`

```swift 
// update
var numbers: Set = [1, 2, 3, 4, 5]
var oldValue = numbers.update(with: 3) // 3
oldValue = numbers.update(with: -1) // nil
```

#### `intersection()`

```swift 
// intersection
// common elements of two groups
let employeeOneProficientLanguages: Set = ["Java", "Kotlin", "C", "Python", "SQL", "Go", "Dart", "JavaScript"]
let employeeTwoProficientLanguages: Set = ["Swift", "Objective-C", "C", "Python", "JavaScript"]
let languagesInCommon = employeeOneProficientLanguages.intersection(employeeTwoProficientLanguages)
print(languagesInCommon) // ["C", "Python", "JavaScript"]
```

#### Union 

```swift 
```

#### `subtracting()`

```swift 
// subtract
let dsaTopicsToStudy: Set = ["Big O Notation", "String", "Array", "Dictionary", "Set", "Character", "CharacterSet", "Stack", "Queue", "Linked List"]
let topicsCompleted: Set = ["Big O Notation", "String", "Array", "Dictionary", "Linked List"]
let topicsRemaining = dsaTopicsToStudy.subtracting(topicsCompleted)
print(topicsRemaining) // ["Queue", "Stack", "CharacterSet", "Character", "Set"]
```

#### `symmetricDifference()`

```swift 
// symmetricDifference
// genres we each uniquely know
let myGenres: Set = ["Soca", "Reggae", "Hip Hop", "Country", "Blues", "Jazz", "Funk", "Zouk"]
let yourGenres: Set = ["Hip Hop", "Reggae", "Folk", "Jazz", "Blues", "Hi-Life", "Techno", "House"]
let genresWeCanTeachEachOther: Set<String> = myGenres.symmetricDifference(yourGenres)
print(genresWeCanTeachEachOther)
```

## Comparing Sets

#### 

## Finding Elements 

#### `contains()`

#### `allSatisfy(Element -> Bool)`

```swift 
let evenNumbers: Set = [2, 4, 6, 8, 10, 12]
let areAllEven = evenNumbers.allSatisfy { $0 % 2 == 0 }
print(areAllEven) // true
```

## `NSOrderedSet` and `NSMutableOrderedSet`

```swift 
let dupes = [1,1,1,2,2,3,3,3,3,4] // array containing duplicates

var unique = NSOrderedSet(array: dupes) // creating a NSOrderedSet from an Array, it will be unique and keep the order of the elements

print(unique) // [1, 2, 3, 4]

// we cannot modify an NSOrderedSet
// however we an use its counterpart NSMutableOrderedSet

let mutableOrderedSet = NSMutableOrderedSet(array: dupes)
mutableOrderedSet.add(5) 
print(mutableOrderedSet)

mutableOrderedSet[mutableOrderedSet.count - 1] // 5,  [1, 2, 3, 4, 5]
```

## Challenges 

#### Challenge 1 - Unique number of occurences

[LeetCode](https://leetcode.com/problems/unique-number-of-occurrences/)

#### Challenge 2 - Contains duplicate

[LeetCode](https://leetcode.com/problems/contains-duplicate/)

#### Challenge 3 - Destination City

[LeetCode](https://leetcode.com/problems/destination-city/)

#### Challenge 4 - Design HashSet

[LeetCode](https://leetcode.com/problems/design-hashset/)

#### Challenge 5 - Pangram 

[HackerRank](https://www.hackerrank.com/challenges/pangrams/problem)

#### Challenge 6 - First unique Character in a String

[LeetCode](https://leetcode.com/problems/first-unique-character-in-a-string/)

#### Challenge 7 - Unique email addresses

[LeetCode](https://leetcode.com/problems/unique-email-addresses/)


## Resources 

1. [Apple documentation - Set](https://developer.apple.com/documentation/swift/set)
2. [Apple documentation - NSOrderedSet](https://developer.apple.com/documentation/foundation/nsorderedset)
3. [Apple documentation - NSMutableOrderedSet](https://developer.apple.com/documentation/foundation/nsmutableorderedset)
