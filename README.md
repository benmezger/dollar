# $

`$` handles pasting and executing a command copied from the internet. Many
command-line examples are represented with a `$`, which requires you to remove
the first argument (`$`) before executing. This fixes this issue and allows
copy-paste-and-execute without having to worry on removing the dollar sign.

## Installing

Copy `$` to somewhere your `PATH` can find, for example: `/usr/local/bin/`.

## Usage

Copy a command from the internet (be careful!) and paste to your command-line
without removing the `$`.

### Before installing `$`

```sh
$ ls
zsh: command not found: $
$ ls -al
zsh: command not found: $
```

### After installing `$`

```sh
$ ls
$               LICENSE         README.md

$ ls -al
total 24
-rwxr-xr-x   1 seds  staff   136 May  5 09:15 $
drwxr-xr-x   6 seds  staff   192 May  5 09:24 .
drwxr-xr-x  21 seds  staff   672 May  5 08:57 ..
drwxr-xr-x  10 seds  staff   320 May  5 09:25 .git
-rw-r--r--   1 seds  staff  1077 May  5 09:24 LICENSE
-rw-r--r--   1 seds  staff   688 May  5 09:23 README.md

$ whoami
seds

$ who
seds     console  Apr 29 08:46
```
