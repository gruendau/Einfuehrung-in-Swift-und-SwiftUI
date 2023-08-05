---
title: CLI
date: 2023-07-22T20:49:19+02:00
draft: false

subtitle: 

weight: 10

tags: [hugo, cli]
---

## Hugo CLI


Befehle: <br>
[`help`](#hugo-help)
[`completion`](#completion)
[`config`](#config)
[`convert`](#convert)
[`deploy`](#deploy)
[`env`](#env)
[`gen`](#gen)
[`help`](#help)
[`import`](#import)
[`list`](#list)
[`mod`](#mod)
[`new`](#new )
[`server`](#server)
[`version`](#version)

<!--
[``](#)
-->

Hugo CLI-Befehle: <br>
```
  BEFEHL      BESCHREIBUNG
  ----------  ----------------------------------------------------------
  completion  Generate the autocompletion script for the specified shell
  config      Print the site configuration
  convert     Convert your content to different formats
  deploy      Deploy your site to a Cloud provider.
  env         Print Hugo version and environment info
  gen         A collection of several useful generators.
  help        Help about any command
  import      Import your site from others.
  list        Listing out various types of content
  mod         Various Hugo Modules helpers.
  new         Create new content for your site
  server      A high performance webserver
  version     ...
```

##### man hugo

```console
HUGO(1)                            Hugo Manual                           HUGO(1)

NAME
       hugo - hugo builds your site

SYNOPSIS
       hugo [flags]

DESCRIPTION
       hugo is the main command, used to build your Hugo site.

       Hugo is a Fast and Flexible Static Site Generator built with love by
       spf13 and friends in Go.

       Complete documentation is available at https://gohugo.io/.

OPTIONS
       -b, --baseURL=""    
         hostname (and path) to the root, e.g. https://spf13.com/

       -D, --buildDrafts[=false]     
         include content marked as draft

       -E, --buildExpired[=false]    
         include expired content

       -F, --buildFuture[=false]     
         include content with publishdate in the future

       --cacheDir=""  
         filesystem path to cache directory. Defaults: $TMPDIR/hugocache$USER/

       --cleanDestinationDir[=false]      
         remove files from destination not found in static directories

       --clock=""     
         set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00

       --config=""    
         config file (default is hugo.yaml|json|toml)

       --configDir="config"     
         config dir

       -c, --contentDir=""      
         filesystem path to content directory

       --debug[=false]     
         debug output

       -d, --destination=""     
         filesystem path to write files to

       --disableKinds=[]   
         disable different kind of pages (home, RSS etc.)

       --enableGitInfo[=false]  
         add Git revision, date, author, and CODEOWNERS info to the pages

       -e, --environment=""     
         build environment

       --forceSyncStatic[=false]     
         copy all files when static is changed.

       --gc[=false]   
         enable to run some cleanup tasks (remove unused cache
         files) after the build

       -h, --help[=false]  
         help for hugo

       --ignoreCache[=false]    
         ignores the cache directory

       --ignoreVendorPaths=""   
         ignores any _vendor for module paths matching the given Glob pattern

       -l, --layoutDir=""  
         filesystem path to layout directory

       --logLevel=""  
         log level (debug|info|warn|error)

       --minify[=false]    
         minify any supported output format (HTML, XML etc.)

       --noBuildLock[=false]    
         don't create .hugo_build.lock file

       --noChmod[=false]   
         don't sync permission mode of files

       --noTimes[=false]   
         don't sync modification time of files

       --panicOnWarning[=false]      
         panic on first WARNING log

       --poll=""     
         set this to a poll interval, e.g --poll 700ms, to use a
         poll based approach to watch for file system changes

       --printI18nWarnings[=false]   
         print missing translations

       --printMemoryUsage[=false]    
         print memory usage to screen at intervals

       --printPathWarnings[=false]   
         print warnings on duplicate target paths etc.

       --printUnusedTemplates[=false]     
         print warnings on unused templates.

       --quiet[=false]     
         build in quiet mode

       --renderToMemory[=false]      
         render to memory (only useful for benchmark testing)

       -s, --source=""     
         filesystem path to read files relative from

       --templateMetrics[=false]     
         display metrics about template executions

       --templateMetricsHints[=false]     
         calculate some improvement hints when combined with --templateMetrics

       -t, --theme=[]      
         themes to use (located in /themes/THEMENAME/)

       --themesDir=""      
         filesystem path to themes directory

       --trace=""     
         write trace to file (not useful in general)

       -v, --verbose[=false]    
         verbose output

       -w, --watch[=false]      
         watch filesystem for changes and recreate as needed

SEE ALSO
       hugo-completion(1), hugo-config(1), hugo-convert(1), hugo-deploy(1),
       hugo-env(1), hugo-gen(1), hugo-import(1), hugo-list(1), hugo-mod(1),
       hugo-new(1), hugo-server(1), hugo-version(1)
```



##### man hugo-server

```console
HUGO-SERVER(1)                     Hugo Manual                    HUGO-SERVER(1)

NAME
       hugo-server - A high performance webserver

SYNOPSIS
       hugo server [command] [flags]

DESCRIPTION
       Hugo provides its own webserver which builds and serves the site.  While
       hugo server is high performance, it is a webserver with limited options.

       'hugo server' will avoid writing the rendered and served content to disk,
       preferring to store it in memory.

       By default hugo will also watch your files for any changes you make and
       automatically rebuild the site. It will then live reload any open browser
       pages and push the latest content to them. As most Hugo sites are built
       in a fraction of a second, you will be able to save and see your changes
       nearly instantly.

OPTIONS
       --appendPort[=true]     
         append port to baseURL

       -b, --baseURL=""    
         hostname (and path) to the root, 
         e.g. https://spf13.com/

       --bind="127.0.0.1"  
         interface to which the server will bind

       -D, --buildDrafts[=false]    
         include content marked as draft

       -E, --buildExpired[=false]   
         include expired content

       -F, --buildFuture[=false]     
         include content with publishdate in the future

       --cacheDir=""  
         filesystem path to cache directory. 
         Defaults: $TMPDIR/hugocache$USER/

       --cleanDestinationDir[=false]      
         remove files from destination not
         found in static directories

       -c, --contentDir=""      
         filesystem path to content directory

       --disableBrowserError[=false]      
         do not show build errors in the browser

       --disableFastRender[=false]   
         enables full re-renders on changes

       --disableKinds=[]   
         disable different kind of pages (home, RSS etc.)

       --disableLiveReload[=false]  
         watch without enabling live browser reload on rebuild

       --enableGitInfo[=false]  
         add Git revision, date, author, and CODEOWNERS
         info to the pages

       --forceSyncStatic[=false]     copy all files when static is changed.

       --gc[=false]   enable to run some cleanup tasks (remove unused cache
       files) after the build

       -h, --help[=false]  help for server

       --ignoreCache[=false]    
         ignores the cache directory

       -l, --layoutDir=""  
         filesystem path to layout directory

       --liveReloadPort=-1      
         port for live reloading (i.e. 443 in HTTPS proxy situations)

       --meminterval="100ms"    
         interval to poll memory usage (requires --memstats), 
         valid time units are "ns", "us" (or "µs"), "ms", "s", "m", "h".

       --memstats=""  
         log memory usage to this file

       --minify[=false]    
         minify any supported output format (HTML, XML etc.)

       --navigateToChanged[=false]   navigate to changed content file on live
       browser reload

       --noBuildLock[=false]    don't create .hugo_build.lock file

       --noChmod[=false]   don't sync permission mode of files

       --noHTTPCache[=false]    
         prevent HTTP caching

       --noTimes[=false]   
         don't sync modification time of files

       --panicOnWarning[=false]      
         panic on first WARNING log

       --poll=""      
         set this to a poll interval, 
         e.g --poll 700ms, to use a poll based 
         approach to watch for file system changes

       -p, --port=1313     
         port on which the server will listen

       --printI18nWarnings[=false]   
         print missing translations

       --printMemoryUsage[=false]    
         print memory usage to screen at intervals

       --printPathWarnings[=false]   
         print warnings on duplicate target paths etc.

       --printUnusedTemplates[=false]     
         print warnings on unused templates.

       --renderStaticToDisk[=false]  
         serve static files from disk and dynamic
         files from memory

       --renderToDisk[=false]   
         serve all files from disk (default is from memory)

       --templateMetrics[=false]     
         display metrics about template executions

       --templateMetricsHints[=false]     
         calculate some improvement hints when
         combined with --templateMetrics

       -t, --theme=[]      
         themes to use (located in /themes/THEMENAME/)

       --tlsAuto[=false]  
         generate and use locally-trusted certificates.

       --tlsCertFile=""    
         path to TLS certificate file

       --tlsKeyFile=""     
         path to TLS key file

       --trace=""     
         write trace to file (not useful in general)

       -w, --watch[=true]  
         watch filesystem for changes and recreate as needed

OPTIONS INHERITED FROM PARENT COMMANDS
       --clock=""     
         set the clock used by Hugo, 
         e.g. --clock 2021-11-06T22:30:00.00+09:00

       --config=""   
         config file (default is hugo.yaml|json|toml)

       --configDir="config"     
         config dir

       --debug[=false]     
         debug output

       -d, --destination=""     
         filesystem path to write files to

       -e, --environment=""     
         build environment

       --ignoreVendorPaths=""   
         ignores any _vendor for module paths matching
         the given Glob pattern

       --logLevel=""  log level (debug|info|warn|error)

       --quiet[=false]     
         build in quiet mode

       -s, --source=""     
         filesystem path to read files relative from

       --themesDir=""      
         filesystem path to themes directory

       -v, --verbose[=false]    
         verbose output

SEE ALSO
       hugo(1), hugo-server-trust(1)

```



##### man Hugo-new

```console
HUGO-NEW(1)                        Hugo Manual                       HUGO-NEW(1)

NAME
       hugo-new - Create new content for your site

SYNOPSIS
       hugo new [command] [flags]

DESCRIPTION
       Create a new content file and automatically set the date and title.  It
       will guess which kind of file to create based on the path provided.

       You can also specify the kind with -k KIND.

       If archetypes are provided in your theme or site, they will be used.

       Ensure you run this within the root directory of your site.

OPTIONS
       -h, --help[=false]  
         help for new

OPTIONS INHERITED FROM PARENT COMMANDS
       --clock=""     
         set the clock used by Hugo, 
         e.g. --clock 2021-11-06T22:30:00.00+09:00

       --config=""    
         config file (default is hugo.yaml|json|toml)

       --configDir="config"     
         config dir

       --debug[=false]     
         debug output

       -d, --destination=""     
         filesystem path to write files to

       -e, --environment=""     
         build environment

       --ignoreVendorPaths=""   
         ignores any _vendor for module paths matching
         the given Glob pattern

       --logLevel=""  
         log level (debug|info|warn|error)

       --quiet[=false]     
         build in quiet mode

       -s, --source=""     
         filesystem path to read files relative from

       --themesDir=""      
         filesystem path to themes directory

       -v, --verbose[=false]    
         verbose output

SEE ALSO
       hugo(1), hugo-new-content(1), hugo-new-site(1), hugo-new-theme(1)

```



##### hugo help

```console
% hugo --help
hugo is the main command, used to build your Hugo site.

Hugo is a Fast and Flexible Static Site Generator
built with love by spf13 and friends in Go.

Complete documentation is available at https://gohugo.io/.

Usage:
  hugo [flags]
  hugo [command]

Available Commands:
  completion  Generate the autocompletion script for the specified shell
  config      Print the site configuration
  convert     Convert your content to different formats
  deploy      Deploy your site to a Cloud provider.
  env         Print Hugo version and environment info
  gen         A collection of several useful generators.
  help        Help about any command
  import      Import your site from others.
  list        Listing out various types of content
  mod         Various Hugo Modules helpers.
  new         Create new content for your site
  server      A high performance webserver
  version     Print Hugo version and environment info

Flags:
  -b, --baseURL string             hostname (and path) to the root, e.g. https://spf13.com/
  -D, --buildDrafts                include content marked as draft
  -E, --buildExpired               include expired content
  -F, --buildFuture                include content with publishdate in the future
      --cacheDir string            filesystem path to cache directory. Defaults: $TMPDIR/hugo_cache_$USER/
      --cleanDestinationDir        remove files from destination not found in static directories
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              config file (default is hugo.yaml|json|toml)
      --configDir string           config dir (default "config")
  -c, --contentDir string          filesystem path to content directory
      --debug                      debug output
  -d, --destination string         filesystem path to write files to
      --disableKinds strings       disable different kind of pages (home, RSS etc.)
      --enableGitInfo              add Git revision, date, author, and CODEOWNERS info to the pages
  -e, --environment string         build environment
      --forceSyncStatic            copy all files when static is changed.
      --gc                         enable to run some cleanup tasks (remove unused cache files) after the build
  -h, --help                       help for hugo
      --ignoreCache                ignores the cache directory
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
  -l, --layoutDir string           filesystem path to layout directory
      --logLevel string            log level (debug|info|warn|error)
      --minify                     minify any supported output format (HTML, XML etc.)
      --noBuildLock                don't create .hugo_build.lock file
      --noChmod                    don't sync permission mode of files
      --noTimes                    don't sync modification time of files
      --panicOnWarning             panic on first WARNING log
      --poll string                set this to a poll interval, e.g --poll 700ms, 
                                   to use a poll based approach to watch for file system changes
      --printI18nWarnings          print missing translations
      --printMemoryUsage           print memory usage to screen at intervals
      --printPathWarnings          print warnings on duplicate target paths etc.
      --printUnusedTemplates       print warnings on unused templates.
      --quiet                      build in quiet mode
      --renderToMemory             render to memory (only useful for benchmark testing)
  -s, --source string              filesystem path to read files relative from
      --templateMetrics            display metrics about template executions
      --templateMetricsHints       calculate some improvement hints when combined with --templateMetrics
  -t, --theme strings              themes to use (located in /themes/THEMENAME/)
      --themesDir string           filesystem path to themes directory
      --trace file                 write trace to file (not useful in general)
  -v, --verbose                    verbose output
  -w, --watch                      watch filesystem for changes and recreate as needed

Use "hugo [command] --help" for more information about a command.
```

[__`rauf`__][top] [__`runter`__][bottom] 

##### completion

```console
% hugo completion --help
Generate the autocompletion script for hugo for the specified shell.
See each sub-command's help for details on how to use the generated script.

Usage:
  hugo completion [command]

Available Commands:
  bash        Generate the autocompletion script for bash
  fish        Generate the autocompletion script for fish
  powershell  Generate the autocompletion script for powershell
  zsh         Generate the autocompletion script for zsh

Flags:
  -h, --help   help for completion

Global Flags:
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              config file (default is hugo.yaml|json|toml)
      --configDir string           config dir (default "config")
      --debug                      debug output
  -d, --destination string         filesystem path to write files to
  -e, --environment string         build environment
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
      --logLevel string            log level (debug|info|warn|error)
      --quiet                      build in quiet mode
  -s, --source string              filesystem path to read files relative from
      --themesDir string           filesystem path to themes directory
  -v, --verbose                    verbose output

Use "hugo completion [command] --help" for more information about a command.
```

[__`rauf`__][top] [__`runter`__][bottom] 

##### config

```console
% hugo config --help
Print the site configuration, both default and custom settings.

Usage:
  hugo config [command] [flags]
  hugo config [command]

Available Commands:
  mounts      Print the configured file mounts

Flags:
  -b, --baseURL string      hostname (and path) to the root, e.g. https://spf13.com/
      --cacheDir string     filesystem path to cache directory. Defaults: $TMPDIR/hugo_cache_$USER/
  -c, --contentDir string   filesystem path to content directory
      --format string       preferred file format (toml, yaml or json) (default "toml")
  -h, --help                help for config
      --lang string         the language to display config for. Defaults to the first language defined.
  -t, --theme strings       themes to use (located in /themes/THEMENAME/)

Global Flags:
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              config file (default is hugo.yaml|json|toml)
      --configDir string           config dir (default "config")
      --debug                      debug output
  -d, --destination string         filesystem path to write files to
  -e, --environment string         build environment
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
      --logLevel string            log level (debug|info|warn|error)
      --quiet                      build in quiet mode
  -s, --source string              filesystem path to read files relative from
      --themesDir string           filesystem path to themes directory
  -v, --verbose                    verbose output

Use "hugo config [command] --help" for more information about a command.
```



#### convert

```console
% hugo convert --help
Convert your content (e.g. front matter) to different formats.

See convert's subcommands toJSON, toTOML and toYAML for more information.

Usage:
  hugo convert [command]

Available Commands:
  toJSON      Convert front matter to JSON
  toTOML      Convert front matter to TOML
  toYAML      Convert front matter to YAML

Flags:
  -h, --help            help for convert
  -o, --output string   filesystem path to write files to
      --unsafe          enable less safe operations, please backup first

Global Flags:
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              config file (default is hugo.yaml|json|toml)
      --configDir string           config dir (default "config")
      --debug                      debug output
  -d, --destination string         filesystem path to write files to
  -e, --environment string         build environment
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
      --logLevel string            log level (debug|info|warn|error)
      --quiet                      build in quiet mode
  -s, --source string              filesystem path to read files relative from
      --themesDir string           filesystem path to themes directory
  -v, --verbose                    verbose output

Use "hugo convert [command] --help" for more information about a command.
````

[__`rauf`__][top] [__`runter`__][bottom] 

##### deploy

```console
% hugo deploy --help
Deploy your site to a Cloud provider.

See https://gohugo.io/hosting-and-deployment/hugo-deploy/ for detailed
documentation.

Usage:
  hugo deploy [flags] [args]

Flags:
      --confirm          ask for confirmation before making changes to the target
      --dryRun           dry run
      --force            force upload of all files
  -h, --help             help for deploy
      --invalidateCDN    invalidate the CDN cache listed in the deployment target (default true)
      --maxDeletes int   maximum # of files to delete, or -1 to disable (default 256)
      --target string    target deployment from deployments section in config file; defaults to the first one
      --workers int      number of workers to transfer files. defaults to 10 (default 10)

Global Flags:
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              config file (default is hugo.yaml|json|toml)
      --configDir string           config dir (default "config")
      --debug                      debug output
  -d, --destination string         filesystem path to write files to
  -e, --environment string         build environment
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
      --logLevel string            log level (debug|info|warn|error)
      --quiet                      build in quiet mode
  -s, --source string              filesystem path to read files relative from
      --themesDir string           filesystem path to themes directory
  -v, --verbose                    verbose output
```



##### env

```console
% hugo env --help
Print Hugo version and environment info. This is useful in Hugo bug reports

Usage:
  hugo env [flags] [args]

Flags:
  -h, --help   help for env

Global Flags:
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              config file (default is hugo.yaml|json|toml)
      --configDir string           config dir (default "config")
      --debug                      debug output
  -d, --destination string         filesystem path to write files to
  -e, --environment string         build environment
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
      --logLevel string            log level (debug|info|warn|error)
      --quiet                      build in quiet mode
  -s, --source string              filesystem path to read files relative from
      --themesDir string           filesystem path to themes directory
  -v, --verbose                    verbose output
```



##### gen

```console
% hugo gen --help
A collection of several useful generators.

Usage:
  hugo gen [command]

Available Commands:
  chromastyles Generate CSS stylesheet for the Chroma code highlighter
  doc          Generate Markdown documentation for the Hugo CLI.
  man          Generate man pages for the Hugo CLI

Flags:
  -h, --help   help for gen

Global Flags:
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              config file (default is hugo.yaml|json|toml)
      --configDir string           config dir (default "config")
      --debug                      debug output
  -d, --destination string         filesystem path to write files to
  -e, --environment string         build environment
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
      --logLevel string            log level (debug|info|warn|error)
      --quiet                      build in quiet mode
  -s, --source string              filesystem path to read files relative from
      --themesDir string           filesystem path to themes directory
  -v, --verbose                    verbose output

Use "hugo gen [command] --help" for more information about a command.
```



##### help

```console
% hugo help --help
Help provides help for any command in the application.
Simply type hugo help [path to command] for full details.

Usage:
  hugo help [command] [flags]

Flags:
  -h, --help   help for help

Global Flags:
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              config file (default is hugo.yaml|json|toml)
      --configDir string           config dir (default "config")
      --debug                      debug output
  -d, --destination string         filesystem path to write files to
  -e, --environment string         build environment
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
      --logLevel string            log level (debug|info|warn|error)
      --quiet                      build in quiet mode
  -s, --source string              filesystem path to read files relative from
      --themesDir string           filesystem path to themes directory
  -v, --verbose                    verbose output
```



##### import

```console
% hugo import --help
Import your site from other web site generators like Jekyll.

Import requires a subcommand, e.g. `hugo import jekyll jekyll_root_path target_path`.

Usage:
  hugo import [command]

Available Commands:
  jekyll      hugo import from Jekyll

Flags:
  -h, --help   help for import

Global Flags:
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              config file (default is hugo.yaml|json|toml)
      --configDir string           config dir (default "config")
      --debug                      debug output
  -d, --destination string         filesystem path to write files to
  -e, --environment string         build environment
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
      --logLevel string            log level (debug|info|warn|error)
      --quiet                      build in quiet mode
  -s, --source string              filesystem path to read files relative from
      --themesDir string           filesystem path to themes directory
  -v, --verbose                    verbose output

Use "hugo import [command] --help" for more information about a command.
```



##### list

```console
% hugo list --help
Listing out various types of content.

List requires a subcommand, e.g. hugo list drafts

Usage:
  hugo list [command]

Available Commands:
  all         List all posts
  drafts      List all drafts
  expired     List all posts already expired
  future      List all posts dated in the future

Flags:
  -h, --help   help for list

Global Flags:
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              config file (default is hugo.yaml|json|toml)
      --configDir string           config dir (default "config")
      --debug                      debug output
  -d, --destination string         filesystem path to write files to
  -e, --environment string         build environment
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
      --logLevel string            log level (debug|info|warn|error)
      --quiet                      build in quiet mode
  -s, --source string              filesystem path to read files relative from
      --themesDir string           filesystem path to themes directory
  -v, --verbose                    verbose output

Use "hugo list [command] --help" for more information about a command.
```



##### mod

```console
% hugo mod --help
Various helpers to help manage the modules in your project's dependency graph.
Most operations here requires a Go version installed on your system (>= Go 1.12) and the relevant VCS client (typically Git).
This is not needed if you only operate on modules inside /themes or if you have vendored them via "hugo mod vendor".


Note that Hugo will always start out by resolving the components defined in the site
configuration, provided by a _vendor directory (if no --ignoreVendorPaths flag provided),
Go Modules, or a folder inside the themes directory, in that order.

See https://gohugo.io/hugo-modules/ for more information.

Usage:
  hugo mod [command]

Available Commands:
  clean       Delete the Hugo Module cache for the current project.
  get         Resolves dependencies in your current Hugo Project.
  graph       Print a module dependency graph.
  init        Initialize this project as a Hugo Module.
  npm         Various npm helpers.
  tidy        Remove unused entries in go.mod and go.sum.
  vendor      Vendor all module dependencies into the _vendor directory.
  verify      Verify dependencies.

Flags:
  -h, --help   help for mod

Global Flags:
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              config file (default is hugo.yaml|json|toml)
      --configDir string           config dir (default "config")
      --debug                      debug output
  -d, --destination string         filesystem path to write files to
  -e, --environment string         build environment
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
      --logLevel string            log level (debug|info|warn|error)
      --quiet                      build in quiet mode
  -s, --source string              filesystem path to read files relative from
      --themesDir string           filesystem path to themes directory
  -v, --verbose                    verbose output

Use "hugo mod [command] --help" for more information about a command.
```



##### new 

```console
% hugo new --help
Create a new content file and automatically set the date and title.
It will guess which kind of file to create based on the path provided.

You can also specify the kind with `-k KIND`.

If archetypes are provided in your theme or site, they will be used.

Ensure you run this within the root directory of your site.

Usage:
  hugo new content [path] [flags]

Flags:
  -b, --baseURL string      hostname (and path) to the root, e.g. https://spf13.com/
      --cacheDir string     filesystem path to cache directory. Defaults: $TMPDIR/hugo_cache_$USER/
  -c, --contentDir string   filesystem path to content directory
      --editor string       edit new content with this editor, if provided
  -f, --force               overwrite file if it already exists
      --format string       preferred file format (toml, yaml or json) (default "toml")
  -h, --help                help for content
  -k, --kind string         content type to create
  -t, --theme strings       themes to use (located in /themes/THEMENAME/)

Global Flags:
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              config file (default is hugo.yaml|json|toml)
      --configDir string           config dir (default "config")
      --debug                      debug output
  -d, --destination string         filesystem path to write files to
  -e, --environment string         build environment
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
      --logLevel string            log level (debug|info|warn|error)
      --quiet                      build in quiet mode
  -s, --source string              filesystem path to read files relative from
      --themesDir string           filesystem path to themes directory
  -v, --verbose                    verbose output
```



##### server

```console
% hugo server --help
Hugo provides its own webserver which builds and serves the site.
While hugo server is high performance, it is a webserver with limited options.

'hugo server' will avoid writing the rendered and served content to disk,
preferring to store it in memory.

By default hugo will also watch your files for any changes you make and
automatically rebuild the site. It will then live reload any open browser pages
and push the latest content to them. As most Hugo sites are built in a fraction
of a second, you will be able to save and see your changes nearly instantly.

Usage:
  hugo server [command] [flags]
  hugo server [command]

Aliases:
  server, serve

Available Commands:
  trust       Install the local CA in the system trust store.

Flags:
      --appendPort             append port to baseURL (default true)
  -b, --baseURL string         hostname (and path) to the root, e.g. https://spf13.com/
      --bind string            interface to which the server will bind (default "127.0.0.1")
  -D, --buildDrafts            include content marked as draft
  -E, --buildExpired           include expired content
  -F, --buildFuture            include content with publishdate in the future
      --cacheDir string        filesystem path to cache directory. Defaults: $TMPDIR/hugo_cache_$USER/
      --cleanDestinationDir    remove files from destination not found in static directories
  -c, --contentDir string      filesystem path to content directory
      --disableBrowserError    do not show build errors in the browser
      --disableFastRender      enables full re-renders on changes
      --disableKinds strings   disable different kind of pages (home, RSS etc.)
      --disableLiveReload      watch without enabling live browser reload on rebuild
      --enableGitInfo          add Git revision, date, author, and CODEOWNERS info to the pages
      --forceSyncStatic        copy all files when static is changed.
      --gc                     enable to run some cleanup tasks (remove unused cache files) after the build
  -h, --help                   help for server
      --ignoreCache            ignores the cache directory
  -l, --layoutDir string       filesystem path to layout directory
      --liveReloadPort int     port for live reloading (i.e. 443 in HTTPS proxy situations) (default -1)
      --meminterval string     interval to poll memory usage (requires --memstats), valid time units are "ns", "us" (or "µs"), "ms", "s", "m", "h". (default "100ms")
      --memstats string        log memory usage to this file
      --minify                 minify any supported output format (HTML, XML etc.)
      --navigateToChanged      navigate to changed content file on live browser reload
      --noBuildLock            don't create .hugo_build.lock file
      --noChmod                don't sync permission mode of files
      --noHTTPCache            prevent HTTP caching
      --noTimes                don't sync modification time of files
      --panicOnWarning         panic on first WARNING log
      --poll string            set this to a poll interval, e.g --poll 700ms, to use a poll based approach to watch for file system changes
  -p, --port int               port on which the server will listen (default 1313)
      --printI18nWarnings      print missing translations
      --printMemoryUsage       print memory usage to screen at intervals
      --printPathWarnings      print warnings on duplicate target paths etc.
      --printUnusedTemplates   print warnings on unused templates.
      --renderStaticToDisk     serve static files from disk and dynamic files from memory
      --renderToDisk           serve all files from disk (default is from memory)
      --templateMetrics        display metrics about template executions
      --templateMetricsHints   calculate some improvement hints when combined with --templateMetrics
  -t, --theme strings          themes to use (located in /themes/THEMENAME/)
      --tlsAuto                generate and use locally-trusted certificates.
      --tlsCertFile string     path to TLS certificate file
      --tlsKeyFile string      path to TLS key file
      --trace file             write trace to file (not useful in general)
  -w, --watch                  watch filesystem for changes and recreate as needed (default true)

Global Flags:
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              config file (default is hugo.yaml|json|toml)
      --configDir string           config dir (default "config")
      --debug                      debug output
  -d, --destination string         filesystem path to write files to
  -e, --environment string         build environment
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
      --logLevel string            log level (debug|info|warn|error)
      --quiet                      build in quiet mode
  -s, --source string              filesystem path to read files relative from
      --themesDir string           filesystem path to themes directory
  -v, --verbose                    verbose output

Use "hugo server [command] --help" for more information about a command.
```



##### version

```console
% hugo version --help
Print Hugo version and environment info. This is useful in Hugo bug reports.

Usage:
  hugo version [flags] [args]

Flags:
  -h, --help   help for version

Global Flags:
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              config file (default is hugo.yaml|json|toml)
      --configDir string           config dir (default "config")
      --debug                      debug output
  -d, --destination string         filesystem path to write files to
  -e, --environment string         build environment
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
      --logLevel string            log level (debug|info|warn|error)
      --quiet                      build in quiet mode
  -s, --source string              filesystem path to read files relative from
      --themesDir string           filesystem path to themes directory
  -v, --verbose                    verbose output
```

