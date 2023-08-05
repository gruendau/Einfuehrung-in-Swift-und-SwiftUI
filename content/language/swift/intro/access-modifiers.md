---
title: Zugriffsmodifizierer
date: 2023-07-22T20:49:19+02:00
draft: false

subtitle: 

weight: 10

tags: [swift, access-modifiers]
---

## Zugriffsmodifizierer

Swift kennt fünf Zugriffsmodifikatoren (access modifiers) [`open`](#open) [`public`](#public) [`internal`](#internal) [`fileprivate`](#fileprivate) und [`private`](#private).

---
### open

`open` erlaubt den Zugriff von außerhalb eines Swift Moduls.   
Mit Vererbung von Klassen und Überschreiben von Eigenschaften und Methoden.

```swift
open struct Person {
    // ...
}
```



---
### public

`public` erlaubt den Zugriff von außerhalb eines Swift Moduls.    
Ohne Vererbung von Klassen und Überschreiben von Eigenschaften und Methoden.

```swift
public struct Person {
    // ...
}
```



---
### internal

`internal` erlaubt den Zugriff innerhalb eines Swift Moduls.   
Es ist der voreingestellte <_default_> Zugriffsmodifikator in Swift.  

```swift
// Beide Strukturen haben die gleichen Zugriffsrechte.

struct Person {
    // ...
}

internal struct Person {
    // ...
}
```

[__`rauf`__][top] [__`runter`__][bottom]

---
### fileprivate

`fileprivate` erlaubt den Zugriff innerhalb der Swift Datei.

```swift
struct Person {
    // Auf die id kann nur innerhalb der Swift Datei zugegriffen werden.
    fileprivate let id: Int
    // Auf die Namen die ohne Zugriffsmodifiziererangabe, per default  
    // 'internal' sind, kann innerhalb des Swift Moduls zugegriffen werden.
    var vorname: String
    var nachname: String
}
```



---
### private

`private` erlaubt den Zugriff innerhalb einer Struktur (class, struct, enum, ...)

```swift
private struct Person {
    // ...
}
```

```swift
struct Person {
    // Auf die id kann nur innerhalb der Struktur zugegriffen werden.
    private let id: Int
    // Auf die Namen die ohne Zugriffsmodifiziererangabe, per default  
    // 'internal' sind, kann innerhalb des Swift Moduls zugegriffen werden.
    var vorname: String
    var nachname: String
}
```