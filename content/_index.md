---
title: "Einleitung"
date: 2023-07-22T18:33:41+02:00
draft: false
subtitle: "Einstiegsseite der Einführung in Swift und SwiftUI"
---

Einführung in die 2014 vorgestellte Programmiersprache **`Swift`** [{w}][w1], die inzwischen **`Objective-C`** [{w}][w2] bei Apple als Hauptprogrammiersprache abgelöst hat und Einführung in das 2019 vorgestellte deklarative GUI[^1] **`SwiftUI`** [{w}][w3], das bei Apple das etablierte GUI **`UIKit`** ergänzt und ablöst. 

<!-- Links -->
[w1]: https://de.wikipedia.org/wiki/Swift_(Programmiersprache) "wikipedia"
[w2]: https://de.wikipedia.org/wiki/Objective-C "wikipedia"
[w3]: https://de.wikipedia.org/wiki/SwiftUI "wikipedia"
[w4]: https://de.wikipedia.org/wiki/Grafische_Benutzeroberfläche "wikipedia"

<!-- Fussnoten -->
[^1]: GUI: Graphical User Interface [{w}][w4]


`Die Seiten werden seit Juni 2023 aufgebaut.`

## Klassen

Eine Klasse <_class_> [{d}][d1] ist ein Typ für referenzierbare Objekte zur Datenkapselung von Eigenschaften <_properties_> und Methoden <_methodes_>. Für die Deklarierung wird das Schlüsselwort `class` genutzt.   

[d1]: https://docs.swift.org/swift-book/documentation/the-swift-programming-language/classesandstructures "swift.org"

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

... und hier geht der Text irgendwie weiter!


Badge 
<div class="badge bg-primary text-wrap" style="width: 6rem;">
    I am a badge
</div>



<!-- Button test -->
<!--
  <a class="btn btn-primary" href="/contact" role="button">Link</a>
-->
