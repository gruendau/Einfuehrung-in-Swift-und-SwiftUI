---
title: Einführung Swift CLI
date: 2023-07-22T20:49:19+02:00
draft: false

subtitle: 

weight: 10

tags: [swift, cli]
---

## Swift CLI

Text ...

```console
weswift(1)                       Swift Documentation                      swift(1)

NAME
       swift -- Safe, fast, and expressive general-purpose programming language

SYNOPSIS
       To invoke the Swift REPL (Read-Eval-Print-Loop):

           swift

       To execute a Swift program:

           swift program.swift <arguments>

       To work with the Swift Package Manager:

           swift build|package|run|test [options] <inputs>

       To invoke the Swift compiler:

           swiftc [options] <inputs>

       A list of supported options is available through the "-help" option:

           swift -help

           swift build -help

           swiftc -help

DESCRIPTION
       Swift is a general-purpose programming language built using a modern
       approach to safety, performance, and software design patterns.

       The goal of the Swift project is to create the best available language
       for uses ranging from systems programming, to mobile and desktop apps,
       scaling up to cloud services. Most importantly, Swift is designed to make
       writing and maintaining correct programs easier for the developer. To
       achieve this goal, we believe that the most obvious way to write Swift
       code must also be:

       Safe. The most obvious way to write code should also behave in a safe
       manner.  Undefined behavior is the enemy of safety, and developer
       mistakes should be caught before software is in production. Opting for
       safety sometimes means Swift will feel strict, but we believe that
       clarity saves time in the long run.

       Fast. Swift is intended as a replacement for C-based languages (C, C++,
       and Objective-C). As such, Swift must be comparable to those languages in
       performance for most tasks. Performance must also be predictable and
       consistent, not just fast in short bursts that require clean-up later.
       There are lots of languages with novel features - being fast is rare.

       Expressive. Swift benefits from decades of advancement in computer
       science to offer syntax that is a joy to use, with modern features
       developers expect. But Swift is never done. We will monitor language
       advancements and embrace what works, continually evolving to make Swift
       even better.

BUGS
       Reporting bugs is a great way for anyone to help improve Swift. The bug
       tracker for Swift, an open-source project, is located at
       <https://bugs.swift.org>.

       If a bug can be reproduced only within an Xcode project or a playground,
       or if the bug is associated with an Apple NDA, please file a report to
       Apple's Feedback Assistant at <https://feedbackassistant.apple.com>
       instead.

SEE ALSO
   HOME PAGE
       <https://swift.org>

   APPLE DEVELOPER RESOURCES
       <https://developer.apple.com/swift/resources>

   CODE REPOSITORIES
       Swift Programming Language at <https://github.com/apple/swift>

       Swift Package Manager at <https://github.com/apple/swift-package-manager>

swift 5.6.1                        2021-11-08                           swift(1)
```

##### swift

```console
% swift --help
2023-07-24 09:53:01.586 xcodebuild[5062:68490] 
  Requested but did not find extension point with identifier 
  Xcode.IDEKit.ExtensionSentinelHostApplications for extension 
  Xcode.DebuggerFoundation.AppExtensionHosts.watchOS of 
  plug-in com.apple.dt.IDEWatchSupportCore
2023-07-24 09:53:01.587 xcodebuild[5062:68490] 
  Requested but did not find extension point with identifier 
  Xcode.IDEKit.ExtensionPointIdentifierToBundleIdentifier for extension      Xcode.DebuggerFoundation.AppExtensionToBundleIdentifierMap.watchOS of 
  plug-in com.apple.dt.IDEWatchSupportCore
2023-07-24 09:53:02.337 xcodebuild[5063:68509] 
  Requested but did not find extension point with identifier 
  Xcode.IDEKit.ExtensionSentinelHostApplications for extension 
  Xcode.DebuggerFoundation.AppExtensionHosts.watchOS of plug-in 
  com.apple.dt.IDEWatchSupportCore
2023-07-24 09:53:02.337 xcodebuild[5063:68509] 
  Requested but did not find extension point with identifier 
  Xcode.IDEKit.ExtensionPointIdentifierToBundleIdentifier for extension  Xcode.DebuggerFoundation.AppExtensionToBundleIdentifierMap.watchOS of plug-in com.apple.dt.IDEWatchSupportCore

OVERVIEW: Swift compiler

USAGE: swift

OPTIONS:
  -access-notes-path <value>
    Specify YAML file to override attributes on Swift declarations in this module
  -assert-config <value>  
    Specify the assert_configuration replacement. Possible values are Debug, Release, Unchecked, DisableReplacement.
  -clang-target <value>   
    Separately set the target we should use for internal Clang instance
  -color-diagnostics      
    Print diagnostics in color
  -continue-building-after-errors
    Continue building, even after errors are encountered
  -coverage-prefix-map <prefix=replacement>
    Remap source paths in coverage info
  -debug-info-format=<value>
     Specify the debug info format type to either 'dwarf' or 'codeview'
  -debug-info-store-invocation
     Emit the compiler invocation in the debug info.
  -debug-prefix-map <prefix=replacement>
     Remap source paths in debug info
  -diagnostic-style <style>
                          The formatting style used when printing diagnostics ('swift' or 'llvm')
  -disable-actor-data-race-checks
                          Disable runtime checks for actor data races
  -disable-autolinking-runtime-compatibility-concurrency
                          Do not use autolinking for the concurrency runtime compatibility library
  -disable-autolinking-runtime-compatibility-dynamic-replacements
                          Do not use autolinking for the dynamic replacement runtime compatibility library
  -disable-autolinking-runtime-compatibility
                          Do not use autolinking for runtime compatibility libraries
  -disable-clang-target   Disable a separately specified target triple for Clang instance to use
  -disable-incremental-imports
                          Disable cross-module incremental build metadata and driver scheduling for Swift modules
  -disable-only-one-dependency-file
                          Disables incremental build optimization that only produces one dependencies file
  -disallow-use-new-driver
                          Disable using new swift-driver
  -D <value>              Marks a conditional compilation flag as true
  -embed-tbd-for-module <value>
                          Embed symbols from the module in the emitted tbd file
  -enable-actor-data-race-checks
                          Emit runtime checks for actor data races
  -enable-experimental-additive-arithmetic-derivation
                          Enable experimental 'AdditiveArithmetic' derived conformances
  -enable-experimental-concise-pound-file
                          Enable experimental concise '#file' identifier
  -enable-experimental-cxx-interop
                          Allow importing C++ modules into Swift (experimental feature)
  -enable-experimental-forward-mode-differentiation
                          Enable experimental forward mode differentiation
  -enable-incremental-imports
                          Enable cross-module incremental build metadata and driver scheduling for Swift modules
  -enable-library-evolution
                          Build the module to allow binary-compatible library evolution
  -enable-only-one-dependency-file
                          Enables incremental build optimization that only produces one dependencies file
  -enforce-exclusivity=<enforcement>
                          Enforce law of exclusivity
  -experimental-cxx-stdlib <value>
                          C++ standard library to use; forwarded to Clang's -stdlib flag
  -framework <value>      Specifies a framework which should be linked against
  -Fsystem <value>        Add directory to system framework search path
  -F <value>              Add directory to framework search path
  -gdwarf-types           Emit full DWARF type info.
  -gline-tables-only      Emit minimal debug info for backtraces only
  -gnone                  Don't emit debug info
  -g                      Emit debug info. This is the preferred setting for debugging with LLDB.
  -help                   Display available options
  -index-store-path <path>
                          Store indexing data to <path>
  -index-unit-output-path <path>
                          Use <path> as the output path in the produced index data.
  -I <value>              Add directory to the import search path
  -j <n>                  Number of commands to execute in parallel
  -libc <value>           libc runtime library to use
  -locale <locale-code>   Choose a language for diagnostic messages
  -localization-path <path>
                          Path to localized diagnostic messages directory
  -L <value>              Add directory to library link search path
  -l <value>              Specifies a library which should be linked against
  -module-abi-name <value>
                          ABI name to use for the contents of this module
  -module-alias <alias_name=underlying_name>
                          If a source file imports or references module <alias_name>, the <underlying_name> is used for the contents of the file
  -module-cache-path <value>
                          Specifies the Clang module cache path
  -module-link-name <value>
                          Library to link against when using this module
  -module-name <value>    Name of the module to build
  -no-color-diagnostics   Do not print diagnostics in color
  -no-warnings-as-errors  Don't treat warnings as errors
  -nostdimport            Don't search the standard library import path for modules
  -num-threads <n>        Enable multi-threading and specify number of threads
  -Onone                  Compile without any optimization
  -Osize                  Compile with optimizations and target small code size
  -Ounchecked             Compile with optimizations and remove runtime safety checks
  -O                      Compile with optimizations
  -prefix-serialized-debugging-options
                          Apply debug prefix mappings to serialized debug info in Swiftmodule files
  -pretty-print           Pretty-print the output JSON
  -print-educational-notes
                          Include educational notes in printed diagnostic output, if available
  -print-target-info      Print target information for the given target <triple>, such as x86_64-apple-macos10.9
  -Rcross-import          Emit a remark if a cross-import of a module is triggered.
  -remove-runtime-asserts Remove runtime safety checks.
  -requirement-machine-abstract-signatures=<value>
                          Control usage of experimental generic signature minimization: 'on', 'off', or 'verify'
  -requirement-machine-inferred-signatures=<value>
                          Control usage of experimental generic signature minimization: 'on', 'off', or 'verify'
  -requirement-machine-protocol-signatures=<value>
                          Control usage of experimental protocol requirement signature minimization: 'on', 'off', or 'verify'
  -requirement-machine=<value>
                          Control usage of experimental generics implementation: 'on', 'off', or 'verify'
  -Rmodule-loading        Emit a remark and file path of each loaded module
  -Rpass-missed=<value>   Report missed transformations by optimization passes whose name matches the given POSIX regular expression
  -Rpass=<value>          Report performed transformations by optimization passes whose name matches the given POSIX regular expression
  -runtime-compatibility-version <value>
                          Link compatibility library for Swift runtime version, or 'none'
  -save-optimization-record-passes <regex>
                          Only include passes which match a specified regular expression in the generated optimization record (by default, include all passes)
  -save-optimization-record-path <value>
                          Specify the file name of any generated optimization record
  -save-optimization-record=<format>
                          Generate an optimization record file in a specific format (default: YAML)
  -save-optimization-record
                          Generate a YAML optimization record file
  -sdk <sdk>              Compile against <sdk>
  -serialize-diagnostics-path <path>
                          Emit a serialized diagnostics file to <path>
  -static-executable      Statically link the executable
  -static-stdlib          Statically link the Swift standard library
  -suppress-warnings      Suppress all warnings
  -swift-isa-ptrauth-mode <mode>
                          Mode for staging isa/super signing. Supported modes are LegacyAndStrip, NewAndStrip and NewAndAuth.
  -swift-ptrauth-mode <mode>
                          Mode for staging pointer authentication. Supported modes are LegacyAndStrip, NewAndStrip and NewAndAuth.
  -swift-version <vers>   Interpret input according to a specific Swift language version number
  -target-cpu <value>     Generate code for a particular CPU variant
  -target-variant <value> Generate 'zippered' code for macCatalyst that can run on the specified variant target triple in addition to the main -target triple
  -target <triple>        Generate code for the given target <triple>, such as x86_64-apple-macos10.9
  -use-ld=<value>         Specifies the linker to be used
  -user-module-version <vers>
                          Module version specified from Swift module authors
  -version                Print version information and exit
  -vfsoverlay <value>     Add directory to VFS overlay file
  -v                      Show commands to run and use verbose output
  -warn-concurrency       Warn about code that is unsafe according to the Swift Concurrency model and will become ill-formed in a future language version
  -warn-implicit-overrides
                          Warn about implicit overrides of protocol members
  -warn-swift3-objc-inference-complete
                          Warn about deprecated @objc inference in Swift 3 for every declaration that will no longer be inferred as @objc in Swift 4
  -warn-swift3-objc-inference-minimal
                          Warn about deprecated @objc inference in Swift 3 based on direct uses of the Objective-C entrypoint
  -warnings-as-errors     Treat warnings as errors
  -working-directory <path>
                          Resolve file paths relative to the specified directory
  -Xcc <arg>              
    Pass <arg> to the C/C++/Objective-C compiler
  -Xlinker <value>        
    Specifies an option which should be passed to the linker

Welcome to Swift!

Subcommands:

  swift build      Build Swift packages
  swift package    Create and work on packages
  swift run        Run a program from a package
  swift test       Run package tests
  swift repl       Experiment with Swift code interactively (default)

  Use `swift --help` for descriptions of available options and flags.

  Use `swift help <subcommand>` for more information about a subcommand.
```
