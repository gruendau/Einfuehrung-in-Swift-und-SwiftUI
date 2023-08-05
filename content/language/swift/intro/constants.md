---
title: Konstanten
date: 2023-07-22T20:49:19+02:00
draft: false

subtitle: 

weight: 10

tags: [swift, constant]
---

## Konstanten
  
[Konstanten](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/thebasics/#Naming-Constants-and-Variables) sind Objekte zur Speicherung von Werten und/oder Funktionen, die nicht geändert werden können. Für die Deklarierung wird das Schlüsselwort 'let' genutzt. 

```swift
// Allgemein
let konstante: Typ = wert    // Die Konstante 'konstante' vom Typ 'Typ' soll den Wert 'wert' haben.
```

```swift
// Beispiel 1
let c1: String = "volker"  
let c2 = "volker"            // Compiler bestimmt den Typ [type inference]
```

```swift
// Beispiel 2a
// Die Konstante 'function' speichert eine Funktion 'gruesse', die als Funktion übergeben wird.
func gruesse () -> String {
    return "hallo"
}
let function: () -> String = gruesse                             // print(function()) --> hallo
```

```swift
// Beispiel 2b
// Die Konstante 'function' speichert eine Funktion 'gruesse', die als Funktion übergeben wird.
func gruesse () -> String {
    return "hallo"
}
let function: () -> String = gruesse                             // print(function()) --> hallo

// Der Compiler bestimmt den Typ [type inference]
let function = gruesse                                           // print(function()) --> hallo
```

```swift
// Beispiel 3a
// Die Konstante 'closure' speichert eine Funktion, die als Closure übergeben wird.
let closure: () -> String = { () -> String in return "hallo" }   // print(closure()) --> hallo
```

```swift
// Beispiel 3b
// Der Compiler bestimmt den Typ [type inference]
let closure: () -> String = { () -> String in return "hallo" }   // print(closure()) --> hallo

// Ohne Typangabe in Closure
let closure: () -> String = { return "hallo" }                   // print(closure()) --> hallo

// Ohne 'return' in Closure
let closure: () -> String = { "hallo" }                          // print(closure()) --> hallo

// Ohne Typangabe für Konstante
let closure = { "hallo" }                                        // print(closure()) --> hallo

// Ohne Closure
let closure = "hallo"                                            // print(closure()) --> hallo
```

<br>

##### Links:

[`buch`](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/thebasics/#Constants-and-Variables, "Swift.org Buch")