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

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git status
On branch dev
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html

no changes added to commit (use "git add" and/or "git commit -a")

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git add .

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   index.html
        modified:   readme.md


belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git stash
Saved working directory and index state WIP on dev: 1e985bf init project

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git stash list
stash@{0}: WIP on dev: 1e985bf init project

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git add about.html

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git stash
Saved working directory and index state WIP on dev: 1e985bf init project

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git add team.html

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git stash
Saved working directory and index state WIP on dev: 1e985bf init project

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git stash list
stash@{0}: WIP on dev: 1e985bf init project
stash@{1}: WIP on dev: 1e985bf init project
stash@{2}: WIP on dev: 1e985bf init project

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (74219c98a9964ae22bd5cf5122a3729530c4bf93)

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git stash list
stash@{0}: WIP on dev: 1e985bf init project
stash@{1}: WIP on dev: 1e985bf init project

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   index.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme.md

Dropped stash@{1} (9095de326c485e945b9d4d48cfb05e343a507d94)

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git add .

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   index.html
        modified:   readme.md


belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git commit -m "setup the home(index) and the about page"
[dev 052c581] setup the home(index) and the about page
 3 files changed, 92 insertions(+)
 create mode 100644 about.html
 create mode 100644 index.html

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git push origin dev
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 1.33 KiB | 226.00 KiB/s, done.
Total 5 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/TimothyBelekollie/git-exercise/pull/new/dev
remote:
To https://github.com/TimothyBelekollie/git-exercise.git
 * [new branch]      dev -> dev

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git stash list
stash@{0}: WIP on dev: 1e985bf init project

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git stash pop stash@{0}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (1f59a44a005a09203fa7350271452e248de15bf1)

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git reset --hard
HEAD is now at 052c581 setup the home(index) and the about page

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$


##Bundle Two


###Exercise One
belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (dev)
$ git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 4 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git pull
Updating 1e985bf..ff34009
Fast-forward
 about.html    |  12 ++++
 index.html    |  12 ++++
 readme.md     | 226 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 services.html |  12 ++++
 4 files changed, 262 insertions(+)
 create mode 100644 about.html
 create mode 100644 index.html
 create mode 100644 services.html
belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme.md
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/service-redesign)
$ git add .

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/service-redesign)
$ git commit -m "changes to services page"
[ft/service-redesign f6dfef9] changes to services page
 2 files changed, 19 insertions(+)

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/service-redesign)
$ git push origin ft/service-redesign
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 706 bytes | 706.00 KiB/s, done.
Total 4 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/TimothyBelekollie/git-exercise/pull/new/ft/service-redesign
remote:
To https://github.com/TimothyBelekollie/git-exercise.git
 * [new branch]      ft/service-redesign -> ft/service-redesign


###EXercise Two

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/service-redesign)
$ git add .

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/service-redesign)
$ git commit -m "new"
[ft/service-redesign f513a72] new
 1 file changed, 2 insertions(+), 1 deletion(-)
belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git add .

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git commit -m "feat: changes to services page"
[main 0a6b8b4] feat: changes to services page
 2 files changed, 11 insertions(+)

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git push origin main
To https://github.com/TimothyBelekollie/git-exercise.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/TimothyBelekollie/git-exercise.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git pull
Auto-merging readme.md
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 799 bytes | 399.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/TimothyBelekollie/git-exercise.git
   4a22b66..604126a  main -> main
   


##Bundle Three

###Exercise One


belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/contact-page)
$ git cherry-pick c5473fa70678eb0faf856a848f6ceb4d6b66a59a
[ft/contact-page d18b3cc] create a team apge
 Date: Mon May 29 12:32:59 2023 +0200
 2 files changed, 19 insertions(+), 1 deletion(-)
 create mode 100644 team.html

 belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page)
$ git status
On branch ft/faq-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

nothing added to commit but untracked files present (use "git add" to track)

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page)
$ git commit -m "feat:creeate faq.html page"
On branch ft/faq-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

nothing added to commit but untracked files present (use "git add" to track)

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page)
$ git add .

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page)
$ git commit -m "feat:creeate faq.html page"
[ft/faq-page 01a578a] feat:creeate faq.html page
 1 file changed, 12 insertions(+)
 create mode 100644 faq.html

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page)
$ git push origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 470 bytes | 470.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/TimothyBelekollie/git-exercise/pull/new/ft/faq-page
remote:
To https://github.com/TimothyBelekollie/git-exercise.git
 * [new branch]      ft/faq-page -> ft/faq-page

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page)
$ git revert c5473fa70678eb0faf856a848f6ceb4d6b66a59a
Auto-merging readme.md
CONFLICT (content): Merge conflict in readme.md
error: could not revert c5473fa... create a team apge
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page|REVERTING)
$ git revert c5473fa70678eb0faf856a848f6ceb4d6b66a59a
error: Reverting is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: revert failed

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page|REVERTING)
$ git revert c5473fa70678eb0faf856a848f6ceb4d6b66a59a
error: Reverting is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: revert failed

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page|REVERTING)
$ git status
On branch ft/faq-page
You are currently reverting commit c5473fa.
  (fix conflicts and run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        deleted:    team.html

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both modified:   readme.md


belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page|REVERTING)
$ git add .

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page|REVERTING)
$ git commit -m "feat: read.me"
[ft/faq-page 9c871c3] feat: read.me
 2 files changed, 4 insertions(+), 14 deletions(-)
 delete mode 100644 team.html

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page)
$ git push origin main
To https://github.com/TimothyBelekollie/git-exercise.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/TimothyBelekollie/git-exercise.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page)
$ git push origin ft/faq-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 367 bytes | 367.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/TimothyBelekollie/git-exercise.git
   01a578a..9c871c3  ft/faq-page -> ft/faq-page



belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page|REVERTING)
$ git add .

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page|REVERTING)
$ git commit -m "final"
[ft/faq-page e83b9e8] final
 1 file changed, 3 insertions(+)
g
belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page)
$ git push origin ft/faq-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 297 bytes | 148.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/TimothyBelekollie/git-exercise.git
   9c871c3..e83b9e8  ft/faq-page -> ft/faq-page

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page)



 parent of c5473fa (create a team apge)

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/team-page)
$ git add .

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/team-page)
$ git commit -m "create a team apge"
[ft/team-page c5473fa] create a team apge
 2 files changed, 19 insertions(+), 1 deletion(-)
 create mode 100644 team.html

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/team-page)
$ git push origin ft/team-page
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 569 bytes | 569.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/TimothyBelekollie/git-exercise/pull/new/ft/team-pag
remote:
To https://github.com/TimothyBelekollie/git-exercise.git
 * [new branch]      ft/team-page -> ft/team-page




###EXercise Two
belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git checkout ft/faq-page
Switched to branch 'ft/faq-page'

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git add .

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git commit -m "feat:changes in index"
[main 2aeeea0] feat:changes in index
 1 file changed, 1 insertion(+), 1 deletion(-)
git
belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 334 bytes | 167.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/TimothyBelekollie/git-exercise.git
   ee2d046..2aeeea0  main -> main

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/home-page-redesign)
$ git rebase main
Current branch ft/home-page-redesign is up to date.


belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/home-page-redesign)
$ git rebase main
Current branch ft/home-page-redesign is up to date.

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/home-page-redesign)
$ git add .

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/home-page-redesign)
$ git commit -m "changes"
[ft/home-page-redesign e326e4b] changes
 2 files changed, 42 insertions(+)
gi
belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/home-page-redesign)
$ git push origin ft/home-page-redesign
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 672 bytes | 672.00 KiB/s, done.
Total 4 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
To https://github.com/TimothyBelekollie/git-exercise.git
   c5a8f1d..e326e4b  ft/home-page-redesign -> ft/home-page-redesign

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 5 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)


belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git checkout ft/faq-page
Switched to branch 'ft/faq-page'

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git add .

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git commit -m "feat:changes in index"
[main 2aeeea0] feat:changes in index
 1 file changed, 1 insertion(+), 1 deletion(-)
git
belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 334 bytes | 167.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/TimothyBelekollie/git-exercise.git
   ee2d046..2aeeea0  main -> main

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/home-page-redesign)
$ git rebase main
Current branch ft/home-page-redesign is up to date.


##Bundle Four

###Exercise One

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git remote add git-copy https://github.com/TimothyBelekollie/git-exercise-clone.git

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git add .

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git commit -m "feat:add changes to the home page"
[main c69465e] feat:add changes to the home page
 1 file changed, 1 insertion(+)

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git push origin
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 362 bytes | 181.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/TimothyBelekollie/git-exercise.git
   9736331..c69465e  main -> main

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git push git-copy
Enumerating objects: 94, done.
Counting objects: 100% (94/94), done.
Delta compression using up to 8 threads
Compressing objects: 100% (93/93), done.
Writing objects: 100% (94/94), 16.23 KiB | 1.16 MiB/s, done.
Total 94 (delta 57), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (57/57), done.
To https://github.com/TimothyBelekollie/git-exercise-clone.git
 * [new branch]      main -> main

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$


###EXercise Two


belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/footer)
$ git add .

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/footer)
$ git commit -m "feat: create a footer page"
[ft/footer 391d029] feat: create a footer page
 1 file changed, 12 insertions(+)
 create mode 100644 footer.html
g
belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/footer)
$ git push origin ft/footer
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 478 bytes | 239.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/TimothyBelekollie/git-exercise/pull/new/ft/footer
remote:
To https://github.com/TimothyBelekollie/git-exercise.git
 * [new branch]      ft/footer -> ft/footer

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/footer)
$ git add .

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/footer)
$ git commit -m "feat:more changes in the footer page"
[ft/footer 37cd552] feat:more changes in the footer page
 1 file changed, 1 insertion(+)

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/footer)
$ git push origin ft/footer
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 380 bytes | 380.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/TimothyBelekollie/git-exercise.git
   391d029..37cd552  ft/footer -> ft/footer

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/footer)
$ git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 2 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (main)
$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/squashing)
$ git merge --squash ft/footer
Updating b1c5b9e..37cd552
Fast-forward
Squash commit -- not updating HEAD
 footer.html | 13 +++++++++++++
 1 file changed, 13 insertions(+)
 create mode 100644 footer.html

belek@TimothyBelekoll MINGW64 ~/Desktop/The GYM Trainership/Week One/Git Exercise-final/git-exercise (ft/squashing)
$ git commit -m "footer changes squashing"
[ft/squashing ed42829] footer changes squashing
 1 file changed, 13 insertions(+)
 create mode 100644 footer.html

##Bundle Four

###EXercise One






###EXercise Two


```


