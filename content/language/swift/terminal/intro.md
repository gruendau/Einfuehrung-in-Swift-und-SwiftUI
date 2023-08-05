---
title: Einführung
date: 2023-07-22T20:49:19+02:00
draft: false

subtitle: 

weight: 10

tags: [swift, terminal]
---

## Swift Programm auf dem Terminal

Der einfachste Weg ein Swift Programm zu erstellen und laufen zu lassen ist das Program in einen Text Editor zu schreiben und dann auf dem Terminal laufen zu lassen.

#### Swift REPL auf dem Terminal: 
  
Das Terminal offen und `swift` eintippen.
Es werden dann einige Angaben zu Swift ausgegeben und nach dem Prompt 1> kann man seinen Programm Code eingeben. Beendet wird Swift REPL durch die Eingabe von `:quit`.

https://ed.com/command-line-swift

```
❯ swift
Apple Swift version 5.6.1 (swiftlang-5.6.0.323.66 clang-1316.0.20.12)
Target: x86_64-apple-macosx12.0

Welcome to Swift!

Subcommands:

  swift build      Build Swift packages
  swift package    Create and work on packages
  swift run        Run a program from a package
  swift test       Run package tests
  swift repl       Experiment with Swift code interactively (default)

  Use `swift --help` for descriptions of available options and flags.

  Use `swift help <subcommand>` for more information about a subcommand.

Welcome to Apple Swift version 5.6.1 (swiftlang-5.6.0.323.66 clang-1316.0.20.12).
Type :help for assistance.
  1> print("hallo swift")
hallo swift
  2> let vorname = "volker"
vorname: String = "volker"
  3> let alter = 17
alter: Int = 17
  4> print(vorname + " ist " + String(alter) + " jahre alt")
volker ist 17 jahre alt
  5> :quit
``` 
