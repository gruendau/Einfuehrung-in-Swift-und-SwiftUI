---
title: Einführung
date: 2023-07-22T20:49:19+02:00
draft: false

subtitle: 

weight: 10

tags: [swift]
---

## Einführung in Swift

Text ...

<!-- Content navigation -->
- [`Konstanten`](#konstanten "constants") 
[`Variablen`](#variablen "variables")
- [`Operatoren`](#operatoren "operators")
[`Numerische Literale`](#numerische-literale "numeric literals")
- [`Zugriffsmodifizierer`](#zugriffsmodifizierer "access modifiers")
- [`Typen`](#typen "types") <br> 
  - [`Einfache Typen`](#einfache-typen "primitive types") 
[`Zeichen`](#zeichen "characters") 
[`Zeichenketten`](#zeichenketten "strings") 
[`Optionale Typen`](#optionale-typen "optional types") 
[`Opaque Typen`](#opaque-typen "opaque types")
  - [`Kollektionen`](#kollektionen "collections") 
    - [`Arrays`](#arrays "arrays")
[`Sets`](#sets "sets") 
[`Wörterbücher`](#wörterbücher, "dictionaries") 
- [`Funktionen`](#funktionen, "functions") 
[`Closures`](#closures "closures") 
- [`Aufzählungen`](#aufzählungen "enumerations") 
[`Klassen`](#klassen "classes") 
[`Strukturen`](#strukturen "structs") 
[`Protokolle`](#protokolle "protokols") 
- [`Eigenschaften`](#eigenschaften "properties") 
[`Methoden`](#methoden "methodes") 
[`Indexierung`](#indexierung "subscripts") 
- [`Ablaufkontrolle`](#ablaufkontrolle "flow control") 
  - [`for-in`](#for-in-schleife "for-in loop")
[`while`](#while-schleife "while loop")
[`repeat-while`](#repeat-while-schleife "repeat-while loop")
[`if`](#if-anweisung "if statement")
[`switch`](#switch-anweisung "switch statement")
- [`Optionale Bindung`](#optionale-bindung "optional binding")
- [`Fehler Behandlung`](#fehler-behandlung "error handling")

### Konstanten    
[Konstanten](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/thebasics/#Naming-Constants-and-Variables) <_constants_> sind Objekte zur Speicherung von Werten und/oder Funktionen, die im Programmverlauf nicht mehr geändert werden können. Für die Deklarierung wird das Schlüsselwort `let` genutzt. 

```swift  
let constant = "volker"         
```

[`details`](./swift-intro-constants) [__`rauf`__][top] [__`runter`__][bottom]

---
### Variablen
[Variablen](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/thebasics/#Naming-Constants-and-Variables) <_variables_> sind Objekte zur Speicherung von Werten und/oder Funktionen, die im Programverlauf geändert werden können. Für die Deklarierung wird das Schlüsselwort `var` genutzt.
    
```swift
var variable = "volker" 
```

[`details`](./swift-intro-variables) [__`rauf`__][top] [__`runter`__][bottom]

---
### Operatoren

[`details`](./swift-intro-operators) [__`rauf`__][top] [__`runter`__][bottom]

---
### Numerische Literale

```swift
let decimalInteger =     17       // 17 in dezimaler Notation
let binaryInteger =      0b10001  // 17 in binärer Notation
let octalInteger =       0o21     // 17 in octal Notation
let hexadecimalInteger = 0x11     // 17 in hexadecimaler Notation
```

[`details`](./swift-intro-numeric_literals) [__`rauf`__][top] [__`runter`__][bottom]

---
### Zugriffsmodifizierer
Text

```swift
private var variable = "volker" 
```

[`details`](./swift-intro-access_modifiers) [__`rauf`__][top] [__`runter`__][bottom]

---
### Typen  
[Typen](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/types) <_types_> sind Vorgaben für den Aufbau von Objekten.  

[`details`](./swift-intro-types) [__`rauf`__][top] [__`runter`__][bottom]
  
---  
### Einfache Typen

```swift
let c: Character = "a"
let s: String = "volker"
let b: Bool = true
let i: Int = -1            // positive und negative Ganzzahen
let i8: Int8 = -1          // Ganzzahlen von -128 bis 127 - (Int8, Int16, Int32, Int64, Int)
let u: UInt = 1            // nur positive Ganzzahen
let f: Float = 1.1
let d: Double = 1.1
```

[`details`](./swift-intro-primitive_types) [__`rauf`__][top] [__`runter`__][bottom]

---
### Zeichen  
Text ...  

[`details`](./swift-intro-characters) [__`rauf`__][top] [__`runter`__][bottom]
  
---
### Zeichenketten  
Text ... 

[`details`](./swift-intro-strings) [__`rauf`__][top] [__`runter`__][bottom]
  
---
### Kollektionen 
[Kollektionen](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/collectiontypes) <_collections_> sind Sammlungen von Daten in Listen, wie [`Arrays`](#arrays), [`Sets`](#sets) und [`Dictionaries`](#dictionaries).

[`details`](./swift-intro-collections) [__`rauf`__][top] [__`runter`__][bottom]
    
---
### Arrays 
Ein [Array](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/collectiontypes#Arrays) <_array_> ist eine geordnete Liste von Elementen. Für die Deklarierung wird das Schlüsselwort `array` genutzt.
    
```swift
let array = ["volker", "nils"]
```

[`details`](./swift-intro-arrays) [__`rauf`__][top] [__`runter`__][bottom]

---
### Sets   
Ein [Set](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/collectiontypes#Sets) <_set_> ist eine ungeordnete Liste von unterschiedlichen Elementen. Für die Deklarierung wird das Schlüsselwort `set` genutzt.
    
```swift
let set: Set = ["volker", "nils"]
```

[`details`](./swift-intro-sets) [__`rauf`__][top] [__`runter`__][bottom]

---
### Wörterbücher
Ein [Wörterbuch](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/collectiontypes#Dictionaries) <_dictionary_> ist eine Liste von ungeordneten Schlüssel/Wert <_key_/_value_> Paaren. Für die Deklarierung wird das Schlüsselwort `dictionary` genutzt.
    
```swift
let wörterbuch = [1: "volker", 2: "nils"]
```

[`details`](./swift-intro-dictionaries) [__`rauf`__][top] [__`runter`__][bottom]

---
### Optionale Typen  
Ein [optionaler Type](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/types/#Optional-Type) <_optional type_> ist eine Typ der auch `nil` (nicht) enthalten darf. Für die Deklarierung wird das Suffix _`?`_ der Typenbezeichnung angehängt.
    
```swift
let o1: Optional<String>    //  Optional<Wrapped>
let o2: String!
```
[`details`](./swift-intro-optional_types) [__`rauf`__][top] [__`runter`__][bottom]

---
### Opaque Typen
Ein [opaquer Type](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/opaquetypes/) <_opaque type_> ist ein Typ der sich verhalten soll wie ein zugeordneter Typ. Für die Deklarierung wird das Schlüsselwort `some` der Typenbezeichnung vorangestellt.  

```swift
```

[`details`](./swift-intro-opaque_types) [__`rauf`__][top] [__`runter`__][bottom]

---
### Funktionen   
Eine [Function](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/functions) <_function_> ist eine  Handlungsanweisung. Für die Deklarierung wird das Schlüsselwort `func` genutzt.   

```swift
func gebeNamen () -> String {
    return "volker"
}
```

[`details`](./swift-intro-functions) [__`rauf`__][top] [__`runter`__][bottom]

---
### Closures 
Ein [Closure](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/closures) <_closure_> ist eine Handlungsanweisung.   

```swift
// Funktion vs. Closure
func gruesseFunktion () -> String { "hallo" }     // print(gruesseFunktion()) -> hallo
let gruesseClosure1: () -> String = { "hallo" }   // print(gruesseClosure1()) -> hallo

let gruesseClosure2 = { "hallo" }                 // print(gruesseClosure2()) -> hallo
```

[`details`](./swift-intro-closures) [__`rauf`__][top] [__`runter`__][bottom]

---
### Aufzählungen
Eine [Aufzählung](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/enumerations) <_enumeration_> ist eine Aufzählung von Werten. Für die Deklarierung wird das Schlüsselwort `enum` genutzt.  

```swift
enum EineAufzählung {
    // Definition des Inhalts der Aufzählung
}
```

[`details`](./swift-intro-enumerations) [__`rauf`__][top] [__`runter`__][bottom]

---
### Klassen
Eine [Klasse](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/classesandstructures) <_class_> ist ein Typ für referenzierbare Objekte zur Datenkapselung von Eigenschaften <_properties_> und Methoden <_methodes_>. Für die Deklarierung wird das Schlüsselwort `class` genutzt.    

```swift
class EineKlasse {
    // Definition des Inhalts der Klasse
}
```

[`details`](./swift-intro-classes) [__`rauf`__][top] [__`runter`__][bottom]

---
### Strukturen 
Eine [Struktur](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/classesandstructures) <_structure_> ist ein Typ für nicht referenzierbare Objekte zur Datenkapselung von Eigenschaften <_properties_> und Methoden <_methodes_>. Für die Deklarierung wird das Schlüsselwort `struct` genutzt.   

```swift
// Allgemein
struct EineStruktur {
    // Definition des Inhalts der Struktur
}

// Beispiel
struct Person {
    var name: String = "volker"
}
```

[`details`](./swift-intro-structs) [__`rauf`__][top] [__`runter`__][bottom]

---
### Protokolle 
Ein [Protokoll](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/protocols) <_protokol_> bescheibt Anforderungen an benutzerdefinierte Typen die mit dem Protokoll konform gehen sollen. Für die Deklarierung wird das Schlüsselwort `protokol` genutzt.  

```swift
// Allgemein
protocol EinProtokoll {
    // Definition des Inhalts des Protokolls
}

// Beispiel
protocol PersonProtokoll {
    var vorname: String { get set }
    var nachname: String { get set }
    
    func gruesse () -> String
}

// Anwendung
class PersonKlasse: PersonProtokoll {
    var vorname: String = "volker"
    var nachname: String = "kasack"
    
    func gruesse() -> String {
        return "Hallo " + vorname + " " + nachname + "!"
    }
}
let person = PersonKlasse()   // print(person.gruesse()) -> Hallo volker kasack
```

[`details`](./swift-intro-protokols) [__`rauf`__][top] [__`runter`__][bottom]

---
### Eigenschaften 
[Eigenschaften](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/properties) <_properties_> sind Konstanten oder Variablen in Klassen oder Strukturen.    

```swift
```

[`details`](./swift-intro-properties) [__`rauf`__][top] [__`runter`__][bottom]

---
### Methoden 
[Methoden](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/methodes) <_methodes_> sind Funktionen in Klassen oder Strukturen.   

```swift
```

[`details`](./swift-intro-methodes) [__`rauf`__][top] [__`runter`__][bottom]

---
### Indexierung  
[Indexe](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/subscripts) <_subscripts_> sind die Positionen von Elementen in geordneten Listen (Arrays).    

```swift
```

[`details`](./swift-intro-subscripts) [__`rauf`__][top] [__`runter`__][bottom]

---
### Ablaufkontrolle  
[Ablaufkontrolle](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/controlflow) <_control flow_>
```swift
```

[`details`](./swift-intro-control_flow) [__`rauf`__][top] [__`runter`__][bottom]

---
### for-in Schleife
Text
```swift
```

[`details`](./swift-intro-for_in_loops) [__`rauf`__][top] [__`runter`__][bottom]


---
### while Schleife
Text
```swift
```

[`details`](./swift-intro-while_loops) [__`rauf`__][top] [__`runter`__][bottom]

---
### repeat-while-Schleife
Text
```swift
```

[`details`](./swift-intro-repeat-while_loops) [__`rauf`__][top] [__`runter`__][bottom]

---
### if Anweisung
Text
```swift
```

[`details`](./swift-intro-if_statement) [__`rauf`__][top] [__`runter`__][bottom]

---
### switch Anweisung
Text
```swift
```

[`details`](./swift-intro-switch_statement) [__`rauf`__][top] [__`runter`__][bottom]

---
### Optionale Bindung
Text
```swift
```

[`details`](./swift-intro-optional_binding) [__`rauf`__][top] [__`runter`__][bottom]

---
### Fehler Behandlung
In Swift können Funktionen definiert werden, die Fehler <Errors> werfen.
Diese fehlerwerfenden Funktionen werden in do-try-catch Anweisungen verarbeitet.

Fehlerwerfende Funktion:
```swift
func canThrowAnError() throws {
    // die Funktion kann einen Fehler werfen.
}
```

do-try-catch Anweisung:
```swift
do {
    try canThrowAnError()
    // weiter wenn kein Fehler geworfen wurde.
} catch {
    // weiter wenn ein Fehler geworfen wurde.
}
```

[`details`](./swift-intro-error_handling) 
