---
title: Klassen
date: 2023-07-22T20:49:19+02:00
draft: false

subtitle: 

weight: 10

tags: [swift, class]
---

## Klassen

Eine [Klasse](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/classesandstructures) <_class_> ist ein Typ für referenzierbare Objekte zur Datenkapselung von Eigenschaften <_properties_> und Methoden <_methodes_>. Für die Deklarierung wird das Schlüsselwort `class` genutzt.    

```swift
// Allgemein
class EineKlasse {
    // Definition des Inhalts der Klasse
}

// Beispiel
class Person {
    // Property
    var name: String = "volker"
    // Methode
    func gruesse () -> String {
        return "Hallo " + name
    }
}
```