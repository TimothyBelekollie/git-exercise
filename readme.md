#THE GYM GIT EXERCISES DOCS

##Bundle One

###Exercise One
```bash

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final
$ mkdir git-exercise

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final
$ cd git-exercise/

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise
$ git init
Initialized empty Git repository in C:/Users/belek/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise/.git/

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (master)
$ git branch -M main

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ code .

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.md

nothing added to commit but untracked files present (use "git add" to track)

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git add readme.md

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git commit -m "init project"
[main (root-commit) 1e985bf] init project
 1 file changed, 31 insertions(+)
 create mode 100644 readme.md
belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git remote add origin https://github.com/TimothyBelekollie/git-exercise.git

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 314 bytes | 157.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/TimothyBelekollie/git-exercise.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git checkout -b dev
Switched to a new branch 'dev'

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git checkout -b test
Switched to a new branch 'test'

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (test)
$ git checkout dev
Switched to branch 'dev'
M       readme.md

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git branch -D test
Deleted branch test (was 1e985bf).



###Exercise Two

##Bundle Two

###Exercise One


###EXercise Two

##Bundle Three

###Exercise One

###EXercise Two

##Bundle Four

###Exercise One

###EXercise Two


