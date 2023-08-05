---
title: associatedtype
date: 2023-07-22T20:49:19+02:00
draft: false

subtitle: 

tag: [swift, keyword]
---

Ein zugeordneter Typ <_associated type_> kann verwendet werden, um ein Protokoll generisch zu machen. Er wird als generischer Typ für Eigenschaften <_properties_> genutzt. Der zugehörige Typ wird mit dem Schlüsselwort `associatedtype` angegeben.

```swift
// TYPE ist der Platzhalter für den generischen Typ
protocol Store {
    associatedtype TYPE

    var items: [TYPE] { get set }
    mutating func add(item: TYPE)
}

extension Store {
    mutating func add(item: TYPE) {
        items.append(item)
    }
}

struct Shop: Store {
    var items = [String]()
}

var shop = Shop()

shop.add(item: "Book")
shop.add(item: "Car")
```

<br>

##### Links:
<!--   
[`doku`](, "Apple Dokumentation")
-->
[`Generics`](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/generics/#Associated-Types, "Swift.org Buch") _<sub>`by Swift.org`</sub>_   
[`Getting started with associated types in Swift Protocols`](https://www.avanderlee.com/swift/associated-types-protocols) _<sub>`by Antoine von der Lee, 2020`</sub>_  
[`AssociatedType in Swift – A Generic Adventure`](https://holyswift.app/associatedtypes-in-swift-a-generic-adventure) _<sub>`by Leonardo, 2020`</sub>_   
[`What is a protocol associated type?`](https://www.hackingwithswift.com/example-code/language/what-is-a-protocol-associated-type) _<sub>`by Paul Hudson, 2019`</sub>_  
[`Understanding protocol associated types and their constraints`](https://www.hackingwithswift.com/articles/74/understanding-protocol-associated-types-and-their-constraints) _<sub>`by Paul Hudson, 2018`</sub>_  
