Read me


Microsoft Windows [Version 10.0.19044.2604]
(c) Microsoft Corporation. All rights reserved.

C:\Users\Himanshu>cd Desktop/myrepo

C:\Users\Himanshu\Desktop\myrepo>mkdir
The syntax of the command is incorrect.

C:\Users\Himanshu\Desktop\myrepo>dir
 Volume in drive C is OS
 Volume Serial Number is BEBD-9780

 Directory of C:\Users\Himanshu\Desktop\myrepo

07-03-2023  14:44    <DIR>          .
07-03-2023  14:44    <DIR>          ..
07-03-2023  14:44               195 FirstProgram.java
               1 File(s)            195 bytes
               2 Dir(s)  22,786,973,696 bytes free

C:\Users\Himanshu\Desktop\myrepo>git init
Reinitialized existing Git repository in C:/Users/Himanshu/Desktop/myrepo/.git/

C:\Users\Himanshu\Desktop\myrepo>git add README.md

C:\Users\Himanshu\Desktop\myrepo>git commit -m "Initial Commit"
[master ca37b8e] Initial Commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

C:\Users\Himanshu\Desktop\myrepo>git remote add origin git@github.com:himanshuch9422/myrepo.git

C:\Users\Himanshu\Desktop\myrepo>git status
On branch master
nothing to commit, working tree clean

C:\Users\Himanshu\Desktop\myrepo>git log
commit ca37b8ee005b131b4aa9eb5da3e03ee07ada495b (HEAD -> master)
Author: himanshuch9422 <himanshuch9422@gmail.com>
Date:   Tue Mar 7 15:36:57 2023 +0530

    Initial Commit

commit 8b3987eb6769f6abe6d48e1fc0776d6860f7d168
Merge: ab99a8b b7e0d3b
Author: himanshuch9422 <himanshuch9422@gmail.com>
Date:   Mon Mar 6 17:25:22 2023 +0530

    Merge after abort

commit b7e0d3b1425ddb8c7fe244614ed018fed7fec469 (MergeSort)
Author: himanshuch9422 <himanshuch9422@gmail.com>
Date:   Mon Mar 6 17:12:27 2023 +0530

    MergeSort Added in the program

commit ab99a8b63d104c5ca175ea83ab27054317783f0f
Author: himanshuch9422 <himanshuch9422@gmail.com>
Date:   Mon Mar 6 17:08:51 2023 +0530

    QuickSort Added

commit d06666552e391992165e6fa44783c82c9f1e2403
Author: himanshuch9422 <himanshuch9422@gmail.com>
Date:   Mon Mar 6 14:05:12 2023 +0530

    Added one print statement

commit 59c99fec95b1ffed8a545b99e75367db701ecb74
Author: himanshuch9422 <himanshuch9422@gmail.com>
Date:   Mon Mar 6 14:00:17 2023 +0530

    init FirstProgram.java

C:\Users\Himanshu\Desktop\myrepo>git status
On branch master
nothing to commit, working tree clean

C:\Users\Himanshu\Desktop\myrepo>git config --global user.name "himanshuch9422"

C:\Users\Himanshu\Desktop\myrepo>git config --global user.email "himanshuch9422@gmail.com"

C:\Users\Himanshu\Desktop\myrepo>git config
usage: git config [<options>]

Config file location
    --global              use global config file
    --system              use system config file
    --local               use repository config file
    --worktree            use per-worktree config file
    -f, --file <file>     use given config file
    --blob <blob-id>      read config from given blob object

Action
    --get                 get value: name [value-pattern]
    --get-all             get all values: key [value-pattern]
    --get-regexp          get values for regexp: name-regex [value-pattern]
    --get-urlmatch        get value specific for the URL: section[.var] URL
    --replace-all         replace all matching variables: name value [value-pattern]
    --add                 add a new variable: name value
    --unset               remove a variable: name [value-pattern]
    --unset-all           remove all matches: name [value-pattern]
    --rename-section      rename section: old-name new-name
    --remove-section      remove a section: name
    -l, --list            list all
    --fixed-value         use string equality when comparing values to 'value-pattern'
    -e, --edit            open an editor
    --get-color           find the color configured: slot [default]
    --get-colorbool       find the color setting: slot [stdout-is-tty]

Type
    -t, --type <>         value is given this type
    --bool                value is "true" or "false"
    --int                 value is decimal number
    --bool-or-int         value is --bool or --int
    --bool-or-str         value is --bool or string
    --path                value is a path (file or directory name)
    --expiry-date         value is an expiry date

Other
    -z, --null            terminate values with NUL byte
    --name-only           show variable names only
    --includes            respect include directives on lookup
    --show-origin         show origin of config (file, standard input, blob, command line)
    --show-scope          show scope of config (worktree, local, global, system, command)
    --default <value>     with --get, use default value when missing entry


C:\Users\Himanshu\Desktop\myrepo>git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager-core
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
user.name=himanshuch9422
user.email=himanshuch9422@gmail.com
user.nae=Himanshu
filesystem.Oracle Corporation|15.0.1|-1094871168.timestampresolution=999 microseconds
filesystem.Oracle Corporation|15.0.1|-1094871168.minracythreshold=0 nanoseconds
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
core.symlinks=false
core.ignorecase=true
remote.origin.url=git@github.com:himanshuch9422/myrepo.git
remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*

C:\Users\Himanshu\Desktop\myrepo>git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'github.com:himanshuch9422/myrepo.git'

C:\Users\Himanshu\Desktop\myrepo>git push -u origin master
Enumerating objects: 18, done.
Counting objects: 100% (18/18), done.
Delta compression using up to 8 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (18/18), 1.53 KiB | 522.00 KiB/s, done.
Total 18 (delta 5), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (5/5), done.
To github.com:himanshuch9422/myrepo.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

C:\Users\Himanshu\Desktop\myrepo>



















































s