---
title: Sets
date: 2023-07-22T20:49:19+02:00
draft: false

subtitle: 

weight: 10

tags: [swift, set]
---

Ein [Set](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/collectiontypes#Sets) <_set_> ist eine ungeordnete Liste von unterschiedlichen Elementen. Für die Deklarierung wird das Schlüsselwort `set` genutzt.
    
```swift
let set: Set = ["volker", "nils"]  // struct Set<Element : Hashable>
```

```swift
// Definition
@frozen
struct Set<Element> where Element : Hashable
```

<br>

##### Links: 
[`doku`](https://developer.apple.com/documentation/swift/set, "Apple Dokumentation")
[`buch`](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/collectiontypes#Sets, "Swift.org Buch")
[Hashable](https://developer.apple.com/documentation/swift/hashable)