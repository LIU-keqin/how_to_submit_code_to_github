test if git is ready

```shell
git
```

return

```
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone     Clone a repository into a new directory
   init      Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add       Add file contents to the index
   mv        Move or rename a file, a directory, or a symlink
   restore   Restore working tree files
   rm        Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect    Use binary search to find the commit that introduced a bug
   diff      Show changes between commits, commit and working tree, etc
   grep      Print lines matching a pattern
   log       Show commit logs
   show      Show various types of objects
   status    Show the working tree status

grow, mark and tweak your common history
   branch    List, create, or delete branches
   commit    Record changes to the repository
   merge     Join two or more development histories together
   rebase    Reapply commits on top of another base tip
   reset     Reset current HEAD to the specified state
   switch    Switch branches
   tag       Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch     Download objects and refs from another repository
   pull      Fetch from and integrate with another repository or a local branch
   push      Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.
```

get git help

```shell
git -help
```

return

```
unknown option: -help
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]
```

Create my name

```shell
git config --global user.name "Liu KQ"
```

Create my email

```shell
git config --global user.email "15991951922@163.com"
```

create a new filefolder

```shell
mkdir scRNA-seq_practice
cd scRNA-seq_practice
```

Synchronization with the service

```shell
git init
```

return

```
Initialized empty Git repository in /Users/keqinliu/scRNA-seq_practice/.git/
```

Then put the code file to commit into a new folder.

git add code file

```shell
git add scRNA-seq_by_seurat_rotationwork.md
```

git commit code description

```shell
git commit -m "It's a practice."
```

return

```
[master (root-commit) c284f91] It's a practice.'
 1 file changed, 358 insertions(+)
 create mode 100644 scRNA-seq_by_seurat_rotationwork.md
```

then submit code

```shell
git remote add origin https://github.com/LIU-keqin/scRNA-seq_practice-.git
git branch -M main
git push -u origin main
```

Then input user name and code

return

```
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 3.43 KiB | 3.43 MiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/LIU-keqin/scRNA-seq_practice-.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
```

