# ZeroToMastery GitHub

Can publish repositories online. Go to settings in repository and enable GitHub Pages

Create repository

Clone or download- select HTTPS. Copy url. 

Then go to terminal, navigate to folders, then use **git clone** command:

```
Rob@Rob-Laptop MINGW64 ~/Documents/My Websites/zero to mastery/JS
$ ls
'advanced control flow'/   advanced_functions/   advanced_objects/   coding_exe/         ES10/   ES8/         how_js_works/         Loops/                            scope/       units_converter/
 advanced_arrays/          advanced_loops/       bground_gen/        DOM_MANIPULATION/   ES6/    Exercises/   JS_logic_exercises/  'pass by value vs by reference'/   script2.js   Variables

Rob@Rob-Laptop MINGW64 ~/Documents/My Websites/zero to mastery/JS
$ cd bground_gen

Rob@Rob-Laptop MINGW64 ~/Documents/My Websites/zero to mastery/JS/bground_gen
$ pwd
/c/Users/rob.OSCDUBAI/Documents/My Websites/zero to mastery/JS/bground_gen

Rob@Rob-Laptop MINGW64 ~/Documents/My Websites/zero to mastery/JS/bground_gen
$ ls
index.html  script.js  style.css

Rob@Rob-Laptop MINGW64 ~/Documents/My Websites/zero to mastery/JS/bground_gen
**$ git clone https://github.com/robhami/background-generator.git**
Cloning into 'background-generator'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.

Rob@Rob-Laptop MINGW64 ~/Documents/My Websites/zero to mastery/JS/bground_gen
```

THis adds folder called background generator to folders in Windows. The .git file allows communication with GitHub. 
Can now copy and paste code files (index.html  script.js  style.css) and put them into background generator folder that was created when folder cloned. 

```
Rob@Rob-Laptop MINGW64 ~/Documents/My Websites/zero to mastery/JS/bground_gen
$ ls
background-generator/  index.html  script.js  style.css

Rob@Rob-Laptop MINGW64 ~/Documents/My Websites/zero to mastery/JS/bground_gen
$ cd background-generator

Rob@Rob-Laptop MINGW64 ~/Documents/My Websites/zero to mastery/JS/bground_gen/background-generator (master)

Rob@Rob-Laptop MINGW64 ~/Documents/My Websites/zero to mastery/JS/bground_gen/background-generator (master)
$ ls
index.html  README.md  script.js  style.css

Rob@Rob-Laptop MINGW64 ~/Documents/My Websites/zero to mastery/JS/bground_gen/background-generator (master)
**$ git status**
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html
        script.js
        style.css

nothing added to commit but untracked files present (use "git add" to track)

```
gits status tells us we have untracked files. Too update them use git add command: 

```
Rob@Rob-Laptop MINGW64 ~/Documents/My Websites/zero to mastery/JS/bground_gen/background-generator (master)
$ git add index.html script.js style.css

Rob@Rob-Laptop MINGW64 ~/Documents/My Websites/zero to mastery/JS/bground_gen/background-generator (master)
$ gits status
bash: gits: command not found

Rob@Rob-Laptop MINGW64 ~/Documents/My Websites/zero to mastery/JS/bground_gen/background-generator (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   index.html
        new file:   script.js
        new file:   style.css
```

Need to now commit, adding a message:

```
Rob@Rob-Laptop MINGW64 ~/Documents/My Websites/zero to mastery/JS/bground_gen/background-generator (master)
$ git commit -m "adding starting project"
[master 18fdb05] adding starting project
 3 files changed, 99 insertions(+)
 create mode 100644 index.html
 create mode 100644 script.js
 create mode 100644 style.css
```

Then we need to push it to the repository: 

```
Rob@Rob-Laptop MINGW64 ~/Documents/My Websites/zero to mastery/JS/bground_gen/background-generator (master)
***$ git push***
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 1.20 KiB | 408.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/robhami/background-generator.git
   dcf97de..18fdb05  master -> master
```