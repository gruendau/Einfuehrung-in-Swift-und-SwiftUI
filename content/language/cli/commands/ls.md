---
title: ls
date: 2023-07-22T20:49:19+02:00
draft: false

subtitle: 

weight: 20

tags: [cli]
---

## ls
Auflistung (ls: 'list') des Inhalts des Verzeichnisses <_directories_>. 

```console
ls [OPTIONS] [FILES]
```

```console
> ls
Desktop
Documents
...
```

### Options
`-l` Lange Liste <_long listing format_>

```console
> ls -l
total 0
drwx------@ 16 test  staff   512 23 Jun 19:31 Desktop
drwx------@ 11 test  staff   352 17 Jun 10:39 Documents
...
```

`-a` Versteckte Dateien anzeigen

```console
> ls -la
total 272
drwxr-xr-x+  37 test  staff   1184 25 Jun 16:39 .
drwxr-xr-x    5 root  admin    160  3 Mai 09:53 ..
...
```
```
Bedeutung des ersten Zeichens:   
-: Regular file  
b: Block special file   
c: Character special file  
d: Directory   
l: Symbolic link  
n: Network file  
p: FIFO   
s: Socket    

Erlaubnisse <_permissions_>:   
r: Permission to read the file  
w: Permission to write to the file   
x: Permission to execute the file   
s: setgid bit   
t: sticky bit   

```


<br>

##### Links:

https://linuxize.com/post/how-to-list-files-in-linux-using-the-ls-command/
