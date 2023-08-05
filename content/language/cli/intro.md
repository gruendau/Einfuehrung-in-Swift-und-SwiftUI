---
title: Einführung
date: 2023-07-22T20:49:19+02:00
draft: false

subtitle: Command Line Interface

weight: 20

tags: [cli]
---

## CLI - Command Line Interface

Bourne shell syntax. Bourne-compatible shells: sh, bash, zsh and ksh

### Befehle

| Befehl | Anmerkung |
| --- | --- |
| [`ls`](./cli-befehl-ls) | ls: 'list' |
| [`alias`](./cli-befehl-alias) |  |
| [`unalias`](./cli-befehl-unalias) |  |
| [`pwd`](./cli-befehl-pwd) | pwd: 'print working directory' |
| [`cd`](./cli-befehl-cd) | cd: 'change directory' |
| [`cp`](./cli-befehl-cp) | cp: 'copy' |
| [`rm`](./cli-befehl-rm) | rm: 'remove directory' |
| [`mv`](./cli-befehl-mv) | mv: 'move' |
| [`mkdir`](./cli-befehl-mkdir) | mkdir: 'make directory' |
| [`man`](./cli-befehl-man) | man: 'manual' |
| [`touch`](./cli-befehl-touch) |  |
| [`chmod`](./cli-befehl-chmod) | chmod: 'change mode' |
| [`./`](./cli-befehl-run-program) | ./: 'run program' |
| [`exit`](./cli-befehl-exit) |  |
| [`sudo`](./cli-befehl-sudo) | sudo: 'superuser do' |
| [`shutdown`](./cli-befehl-shutdown) |  |
| [`htop`](./cli-befehl-htop) |  |
| [`unzip`](./cli-befehl-unzip) |  |
| [`apt`](./cli-befehl-apt) |  |
| [`echo`](./cli-befehl-echo) |  |
| [`cat`](./cli-befehl-cat) | cat: 'concatenate' |
| [`ps`](./cli-befehl-ps) |  |
| [`kill`](./cli-befehl-kill) |  |
| [`ping`](./cli-befehl-ping) |  |
| [`vim`](./cli-befehl-vim) | Open Source Terminal-Texteditor |
| [`history`](./cli-befehl-history) |  |
| [`passwd`](./cli-befehl-passwd) | passwd: 'password' |
| [`which`](./cli-befehl-which) |  |
| [`shred`](./cli-befehl-shred) |  |
| [`less`](./cli-befehl-less) |  |
| [`tail`](./cli-befehl-tail) |  |
| [`head`](./cli-befehl-head) |  |
| [`grep`](./cli-befehl-grep) |  |
| [`whoami`](./cli-befehl-whoami) | whoami: 'who am i' |
| [`whatis`](./cli-befehl-whatis) |  |
| [`wc`](./cli-befehl-wc) | wc: 'word count' |
| [`uname`](./cli-befehl-uname) | uname: 'unix name' |
| [`neofetch`](./cli-befehl-neofetch) |  |
| [`find`](./cli-befehl-find) |  |
| [`wget`](./cli-befehl-wget) | wget: 'world wide web get' Ein Dienstprogramm zum Abrufen von Inhalten aus dem Internet. |

### General Tools

| Befehl | Anmerkung |
| --- | --- |
[`bc`](./cli-befehl-bc) | bc: 'basic calculator' Performs floating point math and various other useful calculations that are not practical with basic shell math support. 
[`expect`](./cli-befehl-expect) | Used to work with hard-to-handle command-line tools that require more complex interaction than is possible with a single pipe. For example, you could use an expect script to interact with getty over a tty or other bidirectional connection to log into a remote computer. In general, scripting that requires two-way interaction between the script and a program is most easily done with an expect script.
[`expr`](./cli-befehl-expr) | Evaluates a numerical expression. This command supports basic integer math, and is frequently used for incrementing a loop iterator.
[`false`](./cli-befehl-false) | Returns a failure exit status (nonzero).
[`sleep`](./cli-befehl-sleep) | Pauses execution for a period of time (measured in seconds). 
[`true`](./cli-befehl-true) | Returns a successful exit status (0).


### Text processing Tools

| Befehl | Anmerkung |
| --- | --- |
[`awk`](./cli-befehl-awk) | Short for Aho, Weinberger, and Kernighan; a programming language in itself, used for text processing using regular expressions. This tool is described further in How AWK-ward. |
[`grep`](./cli-befehl-grep) | Short for Global [search for] Regular Expressions and Print; prints lines matching an input pattern (optionally with a specified number of lines of leading and/or trailing context). The grep command can take input from standard input or from files.Common variants include agrep (“approximate grep” from the Univ. of AZ), fgrep, and egrep.
[`head`](./cli-befehl-head) | Prints the first few lines from a file (or standard input). The number of lines can be specified with the -n flag.
[`perl`](./cli-befehl-perl) | A programming language whose scripts can be easily embedded in shell scripts using the -e flag. Perl's regular expression language is somewhat richer than basic regular expressions (and easier to read than character classes in extended regular expressions), making it popular for text processing use.
[`sed`](./cli-befehl-sed) | Short for stream editor; performs more complex text substitutions using regular expressions.
[`sort`](./cli-befehl-sort) | Sorts a series of lines. By default, sort reads these lines from its standard input. After its standard input is closed, it sorts them and prints the results to its standard output.
[`tail`](./cli-befehl-tail) | Prints the last few lines from of a file (or standard input). The number of lines can be specified with the -n flag. Alternatively, you can specify the starting position as a byte or line offset from either the start or end of the file.
[`tee`](./cli-befehl-tee) | Copies standard input to standard output, saving a copy into a file (or multiple files).
[`tr`](./cli-befehl-tr) | Replaces one character with another.
[`uniq`](./cli-befehl-uniq) | Filters out adjacent lines that match.


### File Commands

| Befehl | Anmerkung |
| --- | --- |
[`cd`](./cli-befehl-cd) | Changes the current working directory. The command cd .. moves up a directory, for example.
[`chflags`](./cli-befehl-chflags) | Changes flags on a file or directory. Most of these flags are relatively obscure. For changing permissions flags, use chmod instead.
[`chgrp`](./cli-befehl-chgrp) | Changes the group ID associated with a file or directory.
[`chmod`](./cli-befehl-chmod) | Changes modes (permission bits) or access control lists (ACLs) on a file or directory.
[`chown`](./cli-befehl-chown) | Changes the ownership of files or directories. This command can also change the group if desired.
[`find`](./cli-befehl-find) | Lists or searches for files in a directory and its subdirectories.
[`ln`](./cli-befehl-ln) | Creates symbolic links and hard links to files or directories.
[`ls`](./cli-befehl-ls) | Lists the files in the current directory.
[`mkdir`](./cli-befehl-mkdir) | Creates new directories.
[`mkfifo`](./cli-befehl-mkfifo) | Creates named pipes for communication. This tool is useful in situations where pipes cannot be established while executing the commands, such as connecting two tools in a circular fashion.
[`mv`](./cli-befehl-mv) | Moves or renames files and directories.
[`rm`](./cli-befehl-rm) [`rmdir`](./cli-befehl-rmdir) | Removes files and directories
[`stat`](./cli-befehl-stat) | Prints detailed file status information, such as the type of file, last modification date, and so on.
[`GetFileInfo`](./cli-befehl-GetFileInfo) [`SetFile`](./cli-befehl-SetFile) | These tools, installed as part of the Developer Tools installation, are useful for getting and manipulating things like extended attributes.Be aware that if you write a script that depends on these, it will require the Developer Tools to be installed.

### Disk Commands

| Befehl | Anmerkung |
| --- | --- |
[`diskutil`](./cli-befehl-diskutil) | Mounts and unmounts volumes and disks, checks disks for consistency, erases optical disks, wipes disks with a security wipe, partitions disks, manipulates RAID sets, and so on.This utility is the command-line counterpart to the Disk Utility application.
[`fsck`](./cli-befehl-fsck) [`fsck_msdos`](./cli-befehl-fsck_msdos) [`fsck_hfs`](./cli-befehl-fsck_hfs) | Checks a file system for consistency.
[`hdiutil`](./cli-befehl-hdiutil)  | Creates and manipulates disk images, including attaching disk images for mounting.
[`mount`](./cli-befehl-mount) [`umount`](./cli-befehl-umount) [`mount_afp`](./cli-befehl-mount_afp) [`mount_cd9660`](./cli-befehl-mount_cd9660)  [`mount_cddafs`](./cli-befehl-mount_cddafs) [`mount_fdesc`](./cli-befehl-mount_fdesc) [`mount_ftp`](./cli-befehl-mount_ftp) [`mount_hfs`](./cli-befehl-mount_hfs) [`mount_msdos`](./cli-befehl-mount_msdos) [`mount_nfs`](./cli-befehl-mount_nfs) [`mount_ntfs`](./cli-befehl-mount_ntfs) [`mount_smbfs`](./cli-befehl-mount_smbfs) [`mount_udf`](./cli-befehl-mount_udf) [`mount_url`](./cli-befehl-mount_url) [`mount_webdav`](./cli-befehl-mount_webdav) | Mounts and unmounts volumes.If you unmount automounted volumes behind the back of the disk arbitration system, you can cause strange behavior in the GUI. Use these commands with care, and if you are trying to unmount an automounted volume, use hdiutil or diskutil instead.


### Archiving and Compression Commands

| Befehl | Anmerkung |
| --- | --- |
[`bzip2`](./cli-befehl-bzip2) [`bunzip2`](./cli-befehl-bunzip2) [`bzip2recover`](./cli-befehl-bzip2recover) | Compresses and decompresses files using the Burrows-Wheeler block sorting text compression algorithm and Huffman coding. This compression tool takes somewhat longer than other tools such as gzip, but tends to result in smaller files, and is thus growing in popularity for distributing large files.Files created with this tool end with the .bz2 extension.
[`compress`](./cli-befehl-uncompress) [`uncompress`](./cli-befehl-uncompress) | Compresses and decompresses files using the Lempel-Ziv-Welsh (LZW) compression algorithm. This compression format has largely fallen out of popularity.Files created by this tool end with the .Z extension.
[`gzip`](./cli-befehl-gzip) [`gunzip`](./cli-befehl-gunzip) [`zcat`](./cli-befehl-zcat) [`gzcat`](./cli-befehl-gzcat) | Compresses, uncompresses, and prints the contents of files in the GNU Zip (LZ77-based) format. This compression scheme is popular with UNIX and Linux users.While based on the same underlying compression scheme, the GNU Zip and ZIP file formats are not the same. The ZIP file format can contain multiple files, while the Gzip file format can only contain a single file (though this single file may be a tar archive).Files created by this tool end with the .gz extension.
[`zip`](./cli-befehl-zip) [`unzip`](./cli-befehl-unzip) [`funzip`](./cli-befehl-funzip) | Compresses and uncompresses files and directories using the ZIP file format (deflate, based on LZ77 and Huffman coding). This file format is commonly used for exchanging compressed files with Windows users.Files created by this tool end with the .zip extension.
[`tar`](./cli-befehl-tar) | Creates, appends to, and extracts multifile archives in the tar (short for “Tape ARchive”) format. This format is the standard format for storing multiple files in a single archive among UNIX and Linux users. The tar file format is usually seen in a compressed form, using either gzip or bzip2.Files created by this tool end with the .tar extension (or the .tgz or .tbz extensions for tar archives compressed with gzip or bzip2).


### xxx

[`awk`](./cli-befehl-awk)

[`bc`](./cli-befehl-bc)
[`bzip2`](./cli-befehl-bzip2) 
[`bunzip2`](./cli-befehl-bunzip2) 
[`bzip2recover`](./cli-befehl-bzip2recover)

[`cd`](./cli-befehl-cd)
[`chflags`](./cli-befehl-chflags) 
[`chgrp`](./cli-befehl-chgrp)
[`chmod`](./cli-befehl-chmod) 
[`chown`](./cli-befehl-chown)
[`compress`](./cli-befehl-uncompress)

[`diskutil`](./cli-befehl-diskutil)

[`expect`](./cli-befehl-expect) 
[`expr`](./cli-befehl-expr)

[`false`](./cli-befehl-false)
[`find`](./cli-befehl-find)
[`fsck`](./cli-befehl-fsck) 
[`fsck_msdos`](./cli-befehl-fsck_msdos) 
[`fsck_hfs`](./cli-befehl-fsck_hfs)
[`funzip`](./cli-befehl-funzip) 

[`GetFileInfo`](./cli-befehl-GetFileInfo)
[`grep`](./cli-befehl-grep)
[`gunzip`](./cli-befehl-gunzip)
[`gzcat`](./cli-befehl-gzcat)
[`gzip`](./cli-befehl-gzip) 
 
[`hdiutil`](./cli-befehl-hdiutil)
[`head`](./cli-befehl-head)

[`ln`](./cli-befehl-ln)
[`ls`](./cli-befehl-ls)

[`mkdir`](./cli-befehl-mkdir)
[`mkfifo`](./cli-befehl-mkfifo)
[`mount`](./cli-befehl-mount) 
[`umount`](./cli-befehl-umount) 
[`mount_afp`](./cli-befehl-mount_afp) 
[`mount_cd9660`](./cli-befehl-mount_cd9660) 
[`mount_cddafs`](./cli-befehl-mount_cddafs) 
[`mount_fdesc`](./cli-befehl-mount_fdesc) 
[`mount_ftp`](./cli-befehl-mount_ftp) 
[`mount_hfs`](./cli-befehl-mount_hfs) 
[`mount_msdos`](./cli-befehl-mount_msdos) 
[`mount_nfs`](./cli-befehl-mount_nfs) 
[`mount_ntfs`](./cli-befehl-mount_ntfs) 
[`mount_smbfs`](./cli-befehl-mount_smbfs) 
[`mount_udf`](./cli-befehl-mount_udf) 
[`mount_url`](./cli-befehl-mount_url) 
[`mount_webdav`](./cli-befehl-mount_webdav)
[`mv`](./cli-befehl-mv)

[`perl`](./cli-befehl-perl)

[`rm`](./cli-befehl-rm) 
[`rmdir`](./cli-befehl-rmdir)

[`sed`](./cli-befehl-sed) 
[`SetFile`](./cli-befehl-SetFile) 
[`sleep`](./cli-befehl-sleep)
[`sort`](./cli-befehl-sort)
[`stat`](./cli-befehl-stat)

[`tail`](./cli-befehl-tail)
[`tar`](./cli-befehl-tar)
[`tee`](./cli-befehl-tee) 
[`tr`](./cli-befehl-tr)
[`true`](./cli-befehl-true) 

[`uncompress`](./cli-befehl-uncompress)
[`uniq`](./cli-befehl-uniq)  
[`unzip`](./cli-befehl-unzip)

[`zcat`](./cli-befehl-zcat) 
[`zip`](./cli-befehl-zip)
 

<!-- xxx -->

### General Tools
[`bc`](./cli-befehl-bc)
[`expect`](./cli-befehl-expect) 
[`expr`](./cli-befehl-expr)
[`false`](./cli-befehl-false)
[`sleep`](./cli-befehl-sleep)
[`true`](./cli-befehl-true) 

### Text processing Tools
[`awk`](./cli-befehl-awk) 
[`grep`](./cli-befehl-grep) 
[`head`](./cli-befehl-head) 
[`perl`](./cli-befehl-perl)
[`sed`](./cli-befehl-sed) 
[`sort`](./cli-befehl-sort)
[`tail`](./cli-befehl-tail)
[`tee`](./cli-befehl-tee) 
[`tr`](./cli-befehl-tr)
[`uniq`](./cli-befehl-uniq) 

### File Commands
[`cd`](./cli-befehl-cd)
[`chflags`](./cli-befehl-chflags) 
[`chgrp`](./cli-befehl-chgrp)
[`chmod`](./cli-befehl-chmod) 
[`chown`](./cli-befehl-chown) 
[`find`](./cli-befehl-find)
[`ln`](./cli-befehl-ln)
[`ls`](./cli-befehl-ls)
[`mkdir`](./cli-befehl-mkdir)
[`mkfifo`](./cli-befehl-mkfifo)
[`mv`](./cli-befehl-mv) 
[`rm`](./cli-befehl-rm) 
[`rmdir`](./cli-befehl-rmdir)
[`stat`](./cli-befehl-stat) 
[`GetFileInfo`](./cli-befehl-GetFileInfo) 
[`SetFile`](./cli-befehl-SetFile) 

### Disk Commands

[`diskutil`](./cli-befehl-diskutil)
[`fsck`](./cli-befehl-fsck) 
[`fsck_msdos`](./cli-befehl-fsck_msdos) 
[`fsck_hfs`](./cli-befehl-fsck_hfs)
[`hdiutil`](./cli-befehl-hdiutil) 
[`mount`](./cli-befehl-mount) 
[`umount`](./cli-befehl-umount) 
[`mount_afp`](./cli-befehl-mount_afp) 
[`mount_cd9660`](./cli-befehl-mount_cd9660) 
[`mount_cddafs`](./cli-befehl-mount_cddafs) 
[`mount_fdesc`](./cli-befehl-mount_fdesc) 
[`mount_ftp`](./cli-befehl-mount_ftp) 
[`mount_hfs`](./cli-befehl-mount_hfs) 
[`mount_msdos`](./cli-befehl-mount_msdos) 
[`mount_nfs`](./cli-befehl-mount_nfs) 
[`mount_ntfs`](./cli-befehl-mount_ntfs) 
[`mount_smbfs`](./cli-befehl-mount_smbfs) 
[`mount_udf`](./cli-befehl-mount_udf) 
[`mount_url`](./cli-befehl-mount_url) 
[`mount_webdav`](./cli-befehl-mount_webdav)

### Archiving and Compression Commands

[`bzip2`](./cli-befehl-bzip2) 
[`bunzip2`](./cli-befehl-bunzip2) 
[`bzip2recover`](./cli-befehl-bzip2recover)
[`compress`](./cli-befehl-uncompress) 
[`uncompress`](./cli-befehl-uncompress) 
[`gzip`](./cli-befehl-gzip) 
[`gunzip`](./cli-befehl-gunzip) 
[`zcat`](./cli-befehl-zcat) 
[`gzcat`](./cli-befehl-gzcat) 
[`zip`](./cli-befehl-zip)
[`unzip`](./cli-befehl-unzip) 
[`funzip`](./cli-befehl-funzip) 
[`tar`](./cli-befehl-tar) 






### Inhalt
- [`alias`](#alias) 
[`apt`](#apt)
- [`cat`](#cat) 
[`cd`](#cd) 
[`chmod`](#chmod)
[`cp`](#cp)
- [`echo`](#echo) 
[`exit`](#exit) 
- [`find`](#find)
- [`grep`](#grep)
- [`head`](#head)
[`history`](#history) 
[`htop`](#htop)
- [`kill`](#kill) 
- [`less`](#less)
[`ls`](#ls) 
- [`man`](#man) 
[`mkdir`](#mkdir)
[`mv`](#mv)
- [`neofetch`](#neofetch)
- [`passwd`](#passwd)
[`ping`](#ping)
[`ps`](#ps)
[`pwd`](#pwd)
- [`rm`](#rm)  
- [`shred`](#shred)
[`shutdown`](#shutdown)
[`sudo`](#sudo)
- [`tail`](#tail)
[`touch`](#touch)
- [`unalias`](#unalias)
[`uname`](#uname)
[`unzip`](#unzip)  
- [`vim`](#vim) 
- [`wc`](#wc)
[`wget`](#wget)
[`whatis`](#whatis)
[`which`](#which) 
[`whoami`](#whoami)
- [`./`](#cli-befehl-run-program)



### alias
Text ...
    
```console
> alias
run-help=man
which-command=whence
```

[`details`](./cli-befehle-alias) [__`rauf`__][top] [__`runter`__][bottom]

---
### apt
Text ...
    
```console
```

[`details`](./cli-befehle-apt) [__`rauf`__][top] [__`runter`__][bottom]

---
### cat
Text ...
    
```console
```

[`details`](./cli-befehle-cat) [__`rauf`__][top] [__`runter`__][bottom]

--- 
### cd
Text ...
    
```console
```

[`details`](./cli-befehle-cd) [__`rauf`__][top] [__`runter`__][bottom]

---
### chmod
Text ...
    
```console
```

[`details`](./cli-befehle-chmod) [__`rauf`__][top] [__`runter`__][bottom]

---
### cp
Text ...
    
```console
```

[`details`](./cli-befehle-) [__`rauf`__][top] [__`runter`__][bottom]

---
### echo
Text ...
    
```console
```

[`details`](./cli-befehle-echo) [__`rauf`__][top] [__`runter`__][bottom]

---
### exit
Text ...
    
```console
```

[`details`](./cli-befehle-exit) [__`rauf`__][top] [__`runter`__][bottom]

---
### find
Text ...
    
```console
```

[`details`](./cli-befehle-find) [__`rauf`__][top] [__`runter`__][bottom]

---
### grep
Text ...
    
```console
```

[`details`](./cli-befehle-grep) [__`rauf`__][top] [__`runter`__][bottom]

---
### head
Text ...
    
```console
```

[`details`](./cli-befehle-head) [__`rauf`__][top] [__`runter`__][bottom]

---
### history
Text ...
    
```console
```

[`details`](./cli-befehle-history) [__`rauf`__][top] [__`runter`__][bottom]

---
### htop
Text ...
    
```console
```

[`details`](./cli-befehle-htop) [__`rauf`__][top] [__`runter`__][bottom]

---
### kill
Text ...
    
```console
```

[`details`](./cli-befehle-kill) [__`rauf`__][top] [__`runter`__][bottom]

---
### less
Text ...
    
```console
```

[`details`](./cli-befehle-less) [__`rauf`__][top] [__`runter`__][bottom]

---
### ls
Text ...
    
```console
```

[`details`](./cli-befehle-ls) [__`rauf`__][top] [__`runter`__][bottom]

---
### man
Text ...
    
```console
```

[`details`](./cli-befehle-man) [__`rauf`__][top] [__`runter`__][bottom]

--- 
### mkdir
Text ...
    
```console
```

[`details`](./cli-befehle-mkdir) [__`rauf`__][top] [__`runter`__][bottom]

---
### mv
Text ...
    
```console
```

[`details`](./cli-befehle-) [__`rauf`__][top] [__`runter`__][bottom]

---
### neofetch
Text ...
    
```console
```

[`details`](./cli-befehle-neofetch) [__`rauf`__][top] [__`runter`__][bottom]

---
### passwd
Text ...
    
```console
```

[`details`](./cli-befehle-passwd) [__`rauf`__][top] [__`runter`__][bottom]

---
### ping
Text ...
    
```console
```

[`details`](./cli-befehle-ping) [__`rauf`__][top] [__`runter`__][bottom]

---
### ps
Text ...
    
```console
```

[`details`](./cli-befehle-ps) [__`rauf`__][top] [__`runter`__][bottom]

---
### pwd
Text ...
    
```console
```

[`details`](./cli-befehle-pwd) [__`rauf`__][top] [__`runter`__][bottom]

---
### rm
Text ...
    
```console
```

[`details`](./cli-befehle-rm) [__`rauf`__][top] [__`runter`__][bottom]

---
### shred
Text ...
    
```console
```

[`details`](./cli-befehle-shred) [__`rauf`__][top] [__`runter`__][bottom]

---
### shutdown
Text ...
    
```console
```

[`details`](./cli-befehle-shutdown) [__`rauf`__][top] [__`runter`__][bottom]

---
### sudo
Text ...
    
```console
```

[`details`](./cli-befehle-sudo) [__`rauf`__][top] [__`runter`__][bottom]

---
### tail
Text ...
    
```console
```

[`details`](./cli-befehle-) [__`rauf`__][top] [__`runter`__][bottom]

---
### touch
Text ...
    
```console
```

[`details`](./cli-befehle-touch) [__`rauf`__][top] [__`runter`__][bottom]

---
### unalias
Text ...
    
```console
```

[`details`](./cli-befehle-unalias) [__`rauf`__][top] [__`runter`__][bottom]

---
### uname
Text ...
    
```console
```

[`details`](./cli-befehle-uname) [__`rauf`__][top] [__`runter`__][bottom]

---
### unzip
Text ...
    
```console
```

[`details`](./cli-befehle-unzip) [__`rauf`__][top] [__`runter`__][bottom]

---
### vim
Text ...
    
```console
```

[`details`](./cli-befehle-vim) [__`rauf`__][top] [__`runter`__][bottom]

---
### wc
Text ...
    
```console
```

[`details`](./cli-befehle-wc) [__`rauf`__][top] [__`runter`__][bottom]

---
### wget
Text ...
    
```console
```

[`details`](./cli-befehle-wget) [__`rauf`__][top] [__`runter`__][bottom]

---
### whatis
Text ...
    
```console
```

[`details`](./cli-befehle-whatis) [__`rauf`__][top] [__`runter`__][bottom]

---
### which
Text ...
    
```console
```

[`details`](./cli-befehle-which) [__`rauf`__][top] [__`runter`__][bottom]

---
### whoami
Text ...
    
```console
```

[`details`](./cli-befehle-whoami) [__`rauf`__][top] [__`runter`__][bottom]

---
### ./
Text ...
    
```console
```

[`details`](./cli-befehle-run_program) [__`rauf`__][top] [__`runter`__][bottom]

<!--
[`alias`](./cli-befehl-alias) 
[`apt`](./cli-befehl-apt)

[`cat`](./cli-befehl-cat) 
[`cd`](./cli-befehl-cd) 
[`chmod`](./cli-befehl-chmod)
[`cp`](./cli-befehl-cp)

[`echo`](./cli-befehl-echo) 
[`exit`](./cli-befehl-exit) 

[`find`](./cli-befehl-find)

[`grep`](./cli-befehl-grep)

[`head`](./cli-befehl-head)
[`history`](./cli-befehl-history) 
[`htop`](./cli-befehl-htop)

[`kill`](./cli-befehl-kill) 

[`less`](./cli-befehl-less)
[`ls`](./cli-befehl-ls) 

[`man`](./cli-befehl-man) 
[`mkdir`](./cli-befehl-mkdir)
[`mv`](./cli-befehl-mv)

[`neofetch`](./cli-befehl-neofetch)

[`passwd`](./cli-befehl-passwd)
[`ping`](./cli-befehl-ping)
[`ps`](./cli-befehl-ps)
[`pwd`](./cli-befehl-pwd)

[`rm`](./cli-befehl-rm)  

[`shred`](./cli-befehl-shred)
[`shutdown`](./cli-befehl-shutdown)
[`sudo`](./cli-befehl-sudo)

[`tail`](./cli-befehl-tail)
[`touch`](./cli-befehl-touch)

[`unalias`](./cli-befehl-unalias)
[`uname`](./cli-befehl-uname)
[`unzip`](./cli-befehl-unzip)  

[`vim`](./cli-befehl-vim) 

[`wc`](./cli-befehl-wc)
[`wget`](./cli-befehl-wget)
[`whatis`](./cli-befehl-whatis)
[`which`](./cli-befehl-which) 
[`whoami`](./cli-befehl-whoami)

[`./`](./cli-befehl-run-program) 
-->


<!-- Content navigation -->
[](#) [](#) [](#)

<!-- ToDos -->
<!-- 
-->

<!--
### CHAPTER

#### SUBCHAPTER
-->

<!-- Program code -->
<!--
```swift
// Programmcode
```
-->

<!-- CONTENT END ############################################## -->

<!-- Comment [__`rauf`__][top] [__`runter`__][bottom] -->

<!-- Links --> <br>
##### Links:
[`Die 40 meist genutzten Linux-Befehle, die du kennen solltest`](https://kinsta.com/de/blog/linux-befehle) _<sub>`von Daniel Diaz, 2023`</sub>_   
[`Kommandozeile (Command Line Interface, CLI)`](https://www.computerweekly.com/de/definition/Kommandozeile-Command-Line-Interface-CLI) _<sub>`von Peter Loshin, 2022`</sub>_
[`Shell Scripting Primer`](https://developer.apple.com/library/archive/documentation/OpenSource/Conceptual/ShellScripting/Introduction/Introduction.html) _<sub>`von apple`</sub>_