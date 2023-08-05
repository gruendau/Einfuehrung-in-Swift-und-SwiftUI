---
title: Wörterbücher
date: 2023-07-22T20:49:19+02:00
draft: false

subtitle: 

weight: 10

tags: [swift, dictionary]
---

Ein [Wörterbuch](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/collectiontypes#Dictionaries) <_dictionary_> ist eine Liste von ungeordneten Schlüssel/Wert <_key_/_value_> Paaren. Für die Deklarierung wird das Schlüsselwort `dictionary` genutzt.
    
```swift
let wörterbuch = [1: "volker", 2: "nils"]   // struct Dictionary<Key : Hashable, Value>
```

```swift
// Definition
@frozen
struct Dictionary<Key, Value> where Key : Hashable
```

```swift
var PersonenDictionary = [1: "volker", 2: "nils", 7: "martin", 5: "Michael"]

for (key, value) in PersonenDictionary {
    print(String(key) + value)
}
```
<br>

##### Links:
[`buch`](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/collectiontypes#Dictionaries, "Swift.org Buch")
[Hashable](https://developer.apple.com/documentation/swift/hashable)
