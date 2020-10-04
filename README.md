# Set

## Initializing a Set
```swift 
// initializing a Set
var babyName: Set<String> = ["Kim", "Hua", "Bertie", "Esther"]
var cohorts: Set = [1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0]
```

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
