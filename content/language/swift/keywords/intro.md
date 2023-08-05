---
title: Einführung
date: 2023-07-22T20:49:19+02:00
draft: false

subtitle: some the "don't care type"

tag: [swift, keyword]
---

## Swift Schlüsselwörter

Schlüsselwörter, die in

- [Deklarationen](#schlüsselwörter-für-deklarationen)
- [Anweisungen](#schlüsselwörter-für-anweisungen) 
- [Ausdrücken und Typen](#schlüsselwörter-für-ausdrücke-und-typen) 
- [Mustern](#schlüsselwörter-für-muster) 
- mit einem [Nummernzeichen](#schlüsselwörter-die-mit-einem-nummernzeichen-(#)-beginnen) (#) beginned
- in bestimmten [Kontexten](#schlüsselwörter-in-bestimmten-kontexten) 

verwendet werden.

### Schlüsselwörter für Deklarationen

| Schlüsselwort | Anmerkung |
| --- | --- |
| [_`associatedtype`_](./swift-keyword-associatedtype) | Ein zugeordneter Typ <_associated type_> kann verwendet werden, um ein Protokoll generisch zu machen. |
| [_`class`_](./swift-keyword-class) |  |
| [_`deinit`_](./swift-keyword-deinit) |  |
| [_`enum`_](./swift-keyword-enum) |  |
| [_`fileprivate`_](./swift-keyword-fileprivate) | Wird als [Zugriffsmodifizierer](./swift-access-modifiers)  <_access modifier_> genutzt. |
| [_`import`_](./swift-keyword-import) |  |
| [_`init`_](./swift-keyword-init) |  |
| [_`inout`_](./swift-keyword-inout) |  |
| [_`internal`_](./swift-keyword-internal) | Wird als [Zugriffsmodifizierer](./swift-access-modifiers)  <_access modifier_> genutzt. |
| [_`let`_](./swift-keyword-let) |  |
| [_`open`_](./swift-keyword-open) | Wird als [Zugriffsmodifizierer](./swift-access-modifiers)  <_access modifier_> genutzt. |
| [_`operator`_](./swift-keyword-operator) |  |
| [_`private`_](./swift-keyword-private) | Wird als [Zugriffsmodifizierer](./swift-access-modifiers)  <_access modifier_> genutzt. |
| [_`public`_](./swift-keyword-public) | Wird als [Zugriffsmodifizierer](./swift-access-modifiers)  <_access modifier_> genutzt. |
| [_`rethrows`_](./swift-keyword-rethrows) |  |
| [_`static`_](./swift-keyword-static) |  |
| [_`struct`_](./swift-keyword-struct) |  |
| [_`subscript`_](./swift-keyword-subscript) |  |
| [_`typealias`_](./swift-keyword-typealias) |  |
| [_`var`_](./swift-keyword-var) |  |

[__`rauf`__][top] [__`runter`__][bottom]

### Schlüsselwörter für Anweisungen

| Schlüsselwort | Anmerkung |
| --- | --- |
| [_`break`_](./swift-keyword-break) | Beendet die Ausführung einer Schleife oder einer `if` oder `switch` Anweisung. |
| [_`case`_](./swift-keyword-case) | Used for pattern testing. |
| [_`catch`_](./swift-keyword-catch) | Behandlung potenzieller Fehler, die durch eine auslösende Funktion `throws` verursacht werden. |
| [_`continue`_](./swift-keyword-continue) | Beendet die Ausführung der aktuellen Iteration einer Schleife, stoppt jedoch nicht die Ausführung der Schleife. |
| [_`default`_](./swift-keyword-default) | Wird für Standardfälle im `switch` verwendet. |
| [_`defer`_](./swift-keyword-defer) | Einen Block vor Beenden einer Funktion ausführen. |
| [_`do`_](./swift-keyword-do) | Wird zum Erstellen von `do` Blöcken verwendet (`do`-`while`, `do`-`catch`). |
| [_`else`_](./swift-keyword-else) | Ausführen eines Blocks, wenn eine Bedingung nicht erfüllt ist. |
| [_`fallthrough`_](./swift-keyword-fallthrough) | ... |
| [_`for`_](./swift-keyword-for) | Durchlaufen einer Sequenz. |
| [_`guard`_](./swift-keyword-guard) | Zustandsbewertung und Entpacken von Optionals. |
| [_`if`_](./swift-keyword-if) | Zustandsbewertung. |
| [_`in`_](./swift-keyword-in) | In closures als Trennzeichen zwischen dem Funktionstyp und dem Funktionskörper und Überprüfung ob sich ein Objekt in einer Sequenz befindet. |
| [_`repeat`_](./swift-keyword-repeat) | A control flow statement, similar to while loop |
| [_`return`_](./swift-keyword-return) | ... |
| [_`throw`_](./swift-keyword-throw) | Auslösen eines Fehlers in einer Funktion, die einen Fehler auslöst `throws`. |
| [_`switch`_](./swift-keyword-switch) | Vergleicht einen Wert mit mehreren möglichen Übereinstimmungsmustern. |
| [_`where`_](./swift-keyword-where) | Herausfiltern von Werten in Anweisungen wie `switch`, `for`, `protocol extension`, `first`, `contains` und `initializers`. |
| [_`while`_](./swift-keyword-while) | Führt eine Schleife aus, bis eine Bedingung `false` wird. |

[__`rauf`__][top] [__`runter`__][bottom]

### Schlüsselwörter für Ausdrücke und Typen

| Schlüsselwort | Anmerkung |
| --- | --- |
| [_`any`_](./swift-keyword-any) | Any can represent an instance of any type at all, including function types. |
| [_`as`_](./swift-keyword-as) | Used for type casting. |
| [_`catch`_](./swift-keyword-catch) | Used in error handling, when an error is thrown, it’s matched against the catch clauses. |
| [_`false`_](./swift-keyword-false) | A literal used to express booleans. |
| [_`is`_](./swift-keyword-is) | Used to check whether an object is of a certain class type |
| [_`nil`_](./swift-keyword-nil) | A valueless state that could be assigned to optionals. |
| [_`rethrows`_](./swift-keyword-rethrows) | allows forwarding a thrown error by a given function parameter |
| [_`self`_](./swift-keyword-self) | “self” refers to the current object within a class or struct. |
| [_`Self`_](./swift-keyword-capitalself) | Refers to a type – usually the current type in the current context. |
| [_`super`_](./swift-keyword-super) | super is used to call up to your superclass. |
| [_`throw`_](./swift-keyword-throw) | Used for throwing an error in a function that throws. |
| [_`throws`_](./swift-keyword-throws) | To mark a function throwing. |
| [_`true`_](./swift-keyword-true) | A literal used to express booleans. |
| [_`try`_](./swift-keyword-try) | The try keyword is used to indicate that a method can throw an error. To catch and handle an error, the throwing method call needs to be wrapped in a do-catch statement. |

[__`rauf`__][top] [__`runter`__][bottom]

### Schlüsselwörter für Muster

| Schlüsselwort | Anmerkung |
| --- | --- |
| [_`-`_](swift-keyword-underscore) |  |

[__`rauf`__][top] [__`runter`__][bottom]

### Schlüsselwörter die mit einem Nummernzeichen (#) beginnen

| Schlüsselwort | Anmerkung |
| --- | --- |
| [_`#available`_](./swift-keyword-hash-available) | Used to determine the availability of APIs at runtime |
| [_`#colorLiteral`_](./swift-keyword-hash-colorLiteral) | Used to make the XCode IDE to display a color swatch 🟥 |
| [_`#column`_](./swift-keyword-hash-column) | column number of the line where it is being run. |
| [_`#dsohandle`_](./swift-keyword-hash-dsohandle) | – |
| [_`#elseif`_](./swift-keyword-hash-elseif) | Literal conditional statement |
| [_`#else`_](./swift-keyword-hash-else) | Literal else statement. |
| [_`#endif`_](./swift-keyword-hash-endif) | Literal marker for closing an a literal if statement |
| [_`#error`_](./swift-keyword-hash-error) | Creates a red compiler error & prevents code from compiling |
| [_`#fileID`_](./swift-keyword-hash-fileid) | Generates concise file string in all language modes. |
| [_`#fileLiteral`_](./swift-keyword-hash-fileliteral) | Used to make the XCode IDE link to a local file. |
| [_`#filePath`_](./swift-keyword-hash-filepath) | Outputs the file path of in which code is being run. |
| [_`#file`_](./swift-keyword-hash-file) | Outputs the name of the file in which code is being run. |
| [_`#function`_](./swift-keyword-hash-function) | Outputs the name of the function where code belongs. |
| [_`#if`_](./swift-keyword-hash-if) | Literal if statement. |
| [_`#imageLiteral`_](./swift-keyword-hash-imageliteral) | Used to make the XCode IDE to display an image. |
| [_`#keyPath`_](./swift-keyword-hash-keypath) | – |
| [_`#line`_](./swift-keyword-hash-line) | line number where it is being run. |
| [_`#selector`_](./swift-keyword-hash-selector) | – |
| [_`#sourceLocation`_](./swift-keyword-hash-sourcelocation) | – |
| [_`#warning`_](./swift-keyword-hash-warning) | will cause Xcode to display a warning with the given message. |

[__`rauf`__][top] [__`runter`__][bottom]

### Schlüsselwörter in bestimmten Kontexten

| Schlüsselwort | Anmerkung |
| --- | --- |
| [_`associativity`_](./swift-keyword-associativity) | defines how operators of the same precedence are grouped together. |
| [_`convenience`_](./swift-keyword-convenience) | Convenience modifier placed before the init keyword. |
| [_`didSet`_](./swift-keyword-didSet) | A property observer |
| [_`dynamic`_](./swift-keyword-dynamic) | A declaration modifier used to make use of Objective-C’s dynamism. |
| [_`final`_](./swift-keyword-final) | One of Swift’s access modifiers. |
| [_`get`_](./swift-keyword-get) | Used when getting a computed property. |
| [_`indirect`_](./swift-keyword-indirect) | Used for recursive Enums |
| [_`infix`_](./swift-keyword-infix) | Used when creating custom operators. |
| [_`lazy`_](./swift-keyword-lazy) | Used for just-in-time calculation. |
| [_`left`_](./swift-keyword-left) | Used to specify the associativity of a custom operator |
| [_`mutating`_](./swift-keyword-mutating) | Functions marked as mutating can change any property within its enclosing value |
| [_`none`_](./swift-keyword-none) | Used to specify the associativity of a custom operator |
| [_`nonmutating`_](./swift-keyword-nonmutating) | – |
| [_`optional`_](./swift-keyword-optional) | – |
| [_`override`_](./swift-keyword-override) | Used for overriding child classes. |
| [_`postfix`_](./swift-keyword-postfix) | Used in creating custom functions, it’s mathematical notation in which operators follow operands. |
| [_`precedence`_](./swift-keyword-precedence) | Operator precedence is a set of rules that determine which operator is executed before another. |
| [_`prefix`_](./swift-keyword-prefix) | Used in creating custom functions, it’s mathematical notation in which operators follow operands. |
| [_`protocol`_](./swift-keyword-protocol) | A protocol defines a blueprint of methods, properties, and other requirements that suit a particular task or piece of functionality. |
| [_`required`_](./swift-keyword-required) | Required keyword means that inheriting classes must provide an implementation of the method. |
| [_`right`_](./swift-keyword-right) | Used to specify the associativity of a custom operator |
| [_`set`_](./swift-keyword-set) | Used when getting a computed property. |
| [_`some`_](./swift-keyword-some) | denotes an opaque type. |
| [_`Type`_](./swift-keyword-Type) | A metatype type refers to the type of any type, including class types, structure types, enumeration types, and protocol types. |
| [_`unowned`_](./swift-keyword-unowned) | A reference type, used for memory management. |
| [_`weak`_](./swift-keyword-weak) | A reference type, used for memory management. |
| [_`willSet`_](./swift-keyword-willSet) | A property observer |

<!-- 
### associatedtype

Ein zugeordneter Typ [associated type] kann verwendet werden, um ein Protokoll generisch zu machen. Der zugehörige Typ wird mit dem Schlüsselwort „associatedtype“ angegeben.

```swift
protocol Store {
    associatedtype WhateverObject

    var items: [WhateverObject] { get set }
    mutating func add(item: WhateverObject)
}

extension Store {
    mutating func add(item: WhateverObject) {
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
___

### class

```swift
```
___

### deinit

```swift
```
___

### enum

```swift
```
___

### fileprivate

```swift
```
___

### import

```swift
```
___

### init

```swift
```
___

### inout

```swift
```
___

### internal

```swift
```
___

### let

```swift
```
___

### open

```swift
```
___

### operator

```swift
```
___

### private

```swift
```
___

### protocol

```swift
```
___

### public

```swift
```
___

### rethrows

```swift
```
___

### static

```swift
```
___

### struct

```swift
```
___

### subscript

```swift
```
___

### typealias

```swift
```
___

### var

```swift
```

-->


https://www.geeksforgeeks.org/swift-keywords/

https://betterprogramming.pub/all-the-reserved-keywords-in-swift-17efcfaa3f3e

https://medium.com/the-traveled-ios-developers-guide/swift-keywords-v-3-0-1-f59783bf26c

[Swift Keywords](https://www.tutorialkart.com/swift-tutorial/swift-keywords/#gsc.tab=0) TutorialKart <br>


<br>

##### Links: 

[`Swift Reserved Keywords, with brief explanations.`](https://swiftbydeya.com/swift-keywords)  _<sub>`von Deya Eldeen, 2022`</sub>_   
[`All the Reserved Keywords in Swift`](https://betterprogramming.pub/all-the-reserved-keywords-in-swift-17efcfaa3f3e) _<sub>`von Artturi Jalli, 2021`</sub>_

