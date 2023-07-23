---
title: "Einleitung"
date: 2023-07-22T18:33:41+02:00
draft: true
subtitle: "Einstiegsseite der Einführung in Swift und SwiftUI"
---

Einführung in die 2014 vorgestellte Programmiersprache [Swift](https://de.wikipedia.org/wiki/Swift_(Programmiersprache)), die inzwischen [Objective-C](https://de.wikipedia.org/wiki/Objective-C) bei Apple als Hauptprogrammiersprache abgelöst hat und Einführung in das 2019 vorgestellte deklarative GUI [SwiftUI](https://de.wikipedia.org/wiki/SwiftUI), das bei Apple das etablierte GUI UIKit ergänzt und ablöst. 

`Die Seiten werden seit Juni 2023 aufgebaut.`

## Klassen

Eine [Klasse](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/classesandstructures "swift.org") <_class_> ist ein Typ für referenzierbare Objekte zur Datenkapselung von Eigenschaften <_properties_> und Methoden <_methodes_>. Für die Deklarierung wird das Schlüsselwort `class` genutzt.    

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

<!-- Button test -->
<!--
  <a class="btn btn-primary" href="/contact" role="button">Link</a>
-->
