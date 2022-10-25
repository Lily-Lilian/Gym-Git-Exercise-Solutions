# Git exercise project

This project will be used for a series of git solution

## bundle 1

### Exercise 1

```bash

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise
$ git init
Initialized empty Git repository in C:/Users/TheGym/Desktop/The Gym/Git-Exercise/.git/

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (master)
$ git branch -M main

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git status
On branch main

No commits yet

nothing to commit (create/copy files and use "git add" to track)

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git status
On branch main

No commits yet

Untracked files:
(use "git add <file>..." to include in what will be committed)
README.md

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git add README.md

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git commit -m "init project"
[main (root-commit) 1941af9] init project
1 file changed, 2 insertions(+)
create mode 100644 README.md

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git remote add origin https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 283 bytes | 283.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git

- [new branch] main -> main
  branch 'main' set up to track 'origin/main'.

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git checkout -b dev
Switched to a new branch 'dev'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (dev)
$ git status
On branch dev
nothing to commit, working tree clean

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (dev)
$ git push origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote: https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions/pull/new/dev
remote:
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git

- [new branch] dev -> dev

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (dev)
$ git checkout -b test
Switched to a new branch 'test'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (test)
$ git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'test' on GitHub by visiting:
remote: https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions/pull/new/test
remote:
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git

- [new branch] test -> test

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (test)
$ git checkout dev
Switched to branch 'dev'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (dev)
$ git branch -D test
Deleted branch test (was 1941af9).

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (dev)
$ git push origin --delete test
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git

- [deleted] test
```

#### Exercises 2

```bash
TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git stash list

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git add home.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git stash
Saved working directory and index state WIP on main: 0abcb4a first exercised

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git stash list
stash@{0}: WIP on main: 0abcb4a first exercised

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git add about.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git stash
Saved working directory and index state WIP on main: 0abcb4a first exercised

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git stash list
stash@{0}: WIP on main: 0abcb4a first exercised
stash@{1}: WIP on main: 0abcb4a first exercised

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git add team.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git stash
Saved working directory and index state WIP on main: 0abcb4a first exercised

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git stash list
stash@{0}: WIP on main: 0abcb4a first exercised
stash@{1}: WIP on main: 0abcb4a first exercised
stash@{2}: WIP on main: 0abcb4a first exercised

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ ^C

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (4fb52364fd49d9ac5e43c86b86e2e3dffe092ae5)

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git stash list
stash@{0}: WIP on main: 0abcb4a first exercised
stash@{1}: WIP on main: 0abcb4a first exercised

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (39176331439c83d5ca0562b8e1b8e4bcc5ed79a0)

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git add --all

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git commit -m "setup the home and about page"
[main 44bea49] setup the home and about page
 2 files changed, 24 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git push origin main
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git remote -v
origin  https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git (fetch)
origin  https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git (push)

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git pull
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 669 bytes | 44.00 KiB/s, done.
From https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions
   0abcb4a..0cc6f4b  main       -> origin/main
Merge made by the 'ort' strategy.
 README.md | 4 ++--
 1 file changed, 2 insertions(+), 2 deletions(-)

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git log
commit 30408f99a762e4124861799d1a74c1ff041b742d (HEAD -> main)
Merge: 44bea49 0cc6f4b
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Mon Oct 24 10:43:40 2022 +0200

    Merge branch 'main' of https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions

commit 44bea496368b07beb128216f7413c8b98a6b542f
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Mon Oct 24 10:39:39 2022 +0200

    setup the home and about page

commit 0cc6f4b048b9e0fdd407394b2a3b8fe945da55d4 (origin/main)
Author: Liliane Iradukunda <98592737+Lily-Lilian@users.noreply.github.com>
Date:   Mon Oct 24 10:09:01 2022 +0200

    Update README.md

commit 0abcb4ab199944f564717918047c16e50ccdcb6a
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Mon Oct 24 10:07:55 2022 +0200

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git push origin main
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 920 bytes | 460.00 KiB/s, done.
Total 6 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git
   0cc6f4b..30408f9  main -> main

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git stash list
stash@{0}: WIP on main: 0abcb4a first exercised

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git stash pop ^C

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git stash pop
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (a30a09e24eefd82b3478160dc8f8a08348da4ffa)

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git reset --hard
HEAD is now at 30408f9 Merge branch 'main' of https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$
```

#### Bundle 2

#### Exercise 1

```bash
TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/bundle-2)
$ git add service.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   service.html


TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/bundle-2)
$ git push origin ft/bundle-2
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/bundle-2)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   service.html


TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git checkout ft/bundle-2
Switched to branch 'ft/bundle-2'
A       service.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   service.html


TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/bundle-2)
$ git commit -m 'added service pages'
[ft/bundle-2 5e8a9c6] added service pages
 1 file changed, 12 insertions(+)
 create mode 100644 service.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/bundle-2)
$ git status
On branch ft/bundle-2
nothing to commit, working tree clean

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/bundle-2)
$ git push origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 470 bytes | 470.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git
   352885d..5e8a9c6  ft/bundle-2 -> ft/bundle-2
```

#### Exercise 2

```bash

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git pull
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (2/2), 700 bytes | 63.00 KiB/s, done.
From https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions
   34d83d5..f11b4ea  main       -> origin/main
Updating 34d83d5..f11b4ea
Fast-forward
 service.html | 12 ++++++++++++
 1 file changed, 12 insertions(+)
 create mode 100644 service.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/service-redesign)
$ git add --all

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   service.html


TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/service-redesign)
$ git commit -m "added services list"
[ft/service-redesign 44762e8] added services list
 1 file changed, 16 insertions(+), 9 deletions(-)

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/service-redesign)
$ git push origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 498 bytes | 498.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git add --all

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git commit -m "added new services"
[main 0dfbf09] added new services
 1 file changed, 15 insertions(+), 9 deletions(-)

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 502 bytes | 502.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git
   f11b4ea..0dfbf09  main -> main

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/service-redesign)
$ git merge main
Auto-merging service.html
CONFLICT (content): Merge conflict in service.html
Automatic merge failed; fix conflicts and then commit the result.

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/service-redesign|MERGING)
$ git add service.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/service-redesign|MERGING)
$ git commit
[ft/service-redesign 55edb8f] Merge branch 'main' into ft/service-redesign

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/service-redesign)
$ git push origin ft/service-redesign
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 431 bytes | 431.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git
   44762e8..55edb8f  ft/service-redesign -> ft/service-redesign
```
