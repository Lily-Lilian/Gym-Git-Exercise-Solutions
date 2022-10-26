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

##### Bundle 3

###### Exercise 1

```bash
TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/team-page)
$ git add team.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/team-page)
$ git status
On branch ft/team-page
Changes to be committed:
 (use "git restore --staged <file>..." to unstage)
       new file:   team.html


TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/team-page)
$ git checkout main
Switched to branch 'main'
M       README.md
A       team.html
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git add README.md

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git commit -m "bundle 2 exercise 2"
[main a61af8c] bundle 2 exercise 2
2 files changed, 128 insertions(+), 1 deletion(-)
create mode 100644 team.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
 (use "git push" to publish your local commits)

nothing to commit, working tree clean

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git push origin main
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1.35 KiB | 690.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git
  0dfbf09..a61af8c  main -> main

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/team-page)
$ git add team.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/team-page)
$ git commit -m "feat:add team page"
[ft/team-page 3244e36] feat:add team page
1 file changed, 12 insertions(+)
create mode 100644 team.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/team-page)
$ git push origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 466 bytes | 466.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git
* [new branch]      ft/team-page -> ft/team-page

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/team-page)
$ git log
commit 3244e362d5545887d34058e31dd3d5c7df4a5b2f (HEAD -> ft/team-page, origin/ft/team-page)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 13:54:03 2022 +0200

   feat:add team page

commit 0dfbf09183bfd099034b20fa4a7b1ec2f8f85f0c
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 12:36:47 2022 +0200

   added new services

commit f11b4eac3b1ab9ffdb469065e90ae6cf735490ce
Merge: 34d83d5 5e8a9c6
Author: Chrissie <chrissiemhrk@gmail.com>
Date:   Tue Oct 25 12:03:47 2022 +0200

   Merge pull request #1 from Lily-Lilian/ft/bundle-2

   added service page

commit 34d83d5db0b98282777e4401f39bec8d77515c3b
:
commit 3244e362d5545887d34058e31dd3d5c7df4a5b2f (HEAD -> ft/team-page, origin/ft/team-page)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 13:54:03 2022 +0200

   feat:add team page

commit 0dfbf09183bfd099034b20fa4a7b1ec2f8f85f0c
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 12:36:47 2022 +0200

   added new services

commit f11b4eac3b1ab9ffdb469065e90ae6cf735490ce
Merge: 34d83d5 5e8a9c6
Author: Chrissie <chrissiemhrk@gmail.com>
Date:   Tue Oct 25 12:03:47 2022 +0200

   Merge pull request #1 from Lily-Lilian/ft/bundle-2

   added service page

commit 34d83d5db0b98282777e4401f39bec8d77515c3b

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/contact-page)
$ git cherry-pick 3244e362d5545887d34058e31dd3d5c7df4a5b2f
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

   git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/contact-page
You are currently cherry-picking commit 3244e36.
 (all conflicts fixed: run "git cherry-pick --continue")
 (use "git cherry-pick --skip" to skip this patch)
 (use "git cherry-pick --abort" to cancel the cherry-pick operation)

nothing to commit, working tree clean

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/contact-page|CHERRY-PICKING)
$ git log
commit a61af8cfa3654b0cf315448359b07c99ac45302c (HEAD -> ft/contact-page, origin/main, main)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 13:44:59 2022 +0200

   bundle 2 exercise 2

commit 0dfbf09183bfd099034b20fa4a7b1ec2f8f85f0c
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 12:36:47 2022 +0200

   added new services

commit f11b4eac3b1ab9ffdb469065e90ae6cf735490ce
Merge: 34d83d5 5e8a9c6
Author: Chrissie <chrissiemhrk@gmail.com>
Date:   Tue Oct 25 12:03:47 2022 +0200

   Merge pull request #1 from Lily-Lilian/ft/bundle-2

   added service page

commit 34d83d5db0b98282777e4401f39bec8d77515c3b

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/contact-page|CHERRY-PICKING)
$ git checkout ft/contact-page
Already on 'ft/contact-page'
warning: cancelling a cherry picking in progress

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/contact-page)
$ git log
commit a61af8cfa3654b0cf315448359b07c99ac45302c (HEAD -> ft/contact-page, origin/main, main)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 13:44:59 2022 +0200

   bundle 2 exercise 2

commit 0dfbf09183bfd099034b20fa4a7b1ec2f8f85f0c
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 12:36:47 2022 +0200

   added new services

commit f11b4eac3b1ab9ffdb469065e90ae6cf735490ce
Merge: 34d83d5 5e8a9c6
Author: Chrissie <chrissiemhrk@gmail.com>
Date:   Tue Oct 25 12:03:47 2022 +0200

   Merge pull request #1 from Lily-Lilian/ft/bundle-2

   added service page

commit 34d83d5db0b98282777e4401f39bec8d77515c3b

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/contact-page)
$ git cherry-pick 3244e362d5545887d34058e31dd3d5c7df4a5b2f
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

   git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/contact-page
You are currently cherry-picking commit 3244e36.
 (all conflicts fixed: run "git cherry-pick --continue")
 (use "git cherry-pick --skip" to skip this patch)
 (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Untracked files:
 (use "git add <file>..." to include in what will be committed)
       contact.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/contact-page|CHERRY-PICKING)
$ git cherry-pick --continue
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

   git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/contact-page
You are currently cherry-picking commit 3244e36.
 (all conflicts fixed: run "git cherry-pick --continue")
 (use "git cherry-pick --skip" to skip this patch)
 (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Untracked files:
 (use "git add <file>..." to include in what will be committed)
       contact.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/contact-page|CHERRY-PICKING)
$ git cherry-pick --skip

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/contact-page)
$ git add contact.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/contact-page)
$ git commit -m "feat:add contact page"
[ft/contact-page a71381f] feat:add contact page
1 file changed, 12 insertions(+)
create mode 100644 contact.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/contact-page)
$ git push origin ft/contact-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 462 bytes | 462.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git
* [new branch]      ft/contact-page -> ft/contact-page

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/faq-page)
$ git add --all

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/faq-page)
$ git commit -m "feat:add faq page"
[ft/faq-page 0023db2] feat:add faq page
1 file changed, 12 insertions(+)
create mode 100644 faq.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/faq-page)
$ git push origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 470 bytes | 470.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git
* [new branch]      ft/faq-page -> ft/faq-page

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/faq-page)
$ git log
commit 0023db20de9fa8d01e263a6c4354b23446886e5f (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 14:27:36 2022 +0200

   feat:add faq page

commit a71381fbd0ef6570459467483d0dbc6ac4107e47 (origin/ft/contact-page, ft/contact-page)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 14:20:25 2022 +0200

   feat:add contact page

commit a61af8cfa3654b0cf315448359b07c99ac45302c (origin/main, main)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 13:44:59 2022 +0200

   bundle 2 exercise 2

commit 0dfbf09183bfd099034b20fa4a7b1ec2f8f85f0c
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 12:36:47 2022 +0200

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/faq-page)
$ git log
commit 0023db20de9fa8d01e263a6c4354b23446886e5f (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 14:27:36 2022 +0200

   feat:add faq page

commit a71381fbd0ef6570459467483d0dbc6ac4107e47 (origin/ft/contact-page, ft/contact-page)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 14:20:25 2022 +0200

   feat:add contact page

commit a61af8cfa3654b0cf315448359b07c99ac45302c (origin/main, main)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 13:44:59 2022 +0200

   bundle 2 exercise 2

commit 0dfbf09183bfd099034b20fa4a7b1ec2f8f85f0c
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 12:36:47 2022 +0200

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/faq-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/team-page)
$ git log
commit 3244e362d5545887d34058e31dd3d5c7df4a5b2f (HEAD -> ft/team-page, origin/ft/team-page)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 13:54:03 2022 +0200

   feat:add team page

commit 0dfbf09183bfd099034b20fa4a7b1ec2f8f85f0c
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 12:36:47 2022 +0200

   added new services

commit f11b4eac3b1ab9ffdb469065e90ae6cf735490ce
Merge: 34d83d5 5e8a9c6
Author: Chrissie <chrissiemhrk@gmail.com>
Date:   Tue Oct 25 12:03:47 2022 +0200

   Merge pull request #1 from Lily-Lilian/ft/bundle-2

   added service page

commit 34d83d5db0b98282777e4401f39bec8d77515c3b

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/team-page)
$ git checkout ft/faq-page
Switched to branch 'ft/faq-page'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/faq-page)
$ git status
On branch ft/faq-page
nothing to commit, working tree clean

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/faq-page)
$ git revert 3244e362d5545887d34058e31dd3d5c7df4a5b2f
[ft/faq-page 193ee96] Revert "feat:add team page"
1 file changed, 12 deletions(-)
delete mode 100644 team.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

   git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/faq-page)
$  git push --set-upstream origin ft/faq-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 277 bytes | 277.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git
  0023db2..193ee96  ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.
```

### Exercise 2

```bash

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git checkout ft/faq-page
Switched to branch 'ft/faq-page'
Your branch is up to date with 'origin/ft/faq-page'.

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git add --all

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git commit -m "feat: added home contents"
[main ab603fc] feat: added home contents
 2 files changed, 9 insertions(+), 20 deletions(-)
 delete mode 100644 team.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/home-page-redesign)
$ git log
commit 193ee9678a310a974ad7a229a5737942ca242740 (HEAD -> ft/home-page-redesign, origin/ft/faq-page, ft/faq-page)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 14:44:00 2022 +0200

    Revert "feat:add team page"

    This reverts commit 3244e362d5545887d34058e31dd3d5c7df4a5b2f.

commit 0023db20de9fa8d01e263a6c4354b23446886e5f
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 14:27:36 2022 +0200

    feat:add faq page

commit a71381fbd0ef6570459467483d0dbc6ac4107e47 (origin/ft/contact-page, ft/contact-page)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 14:20:25 2022 +0200

    feat:add contact page


TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/home-page-redesign)
$ git rebase main
dropping 193ee9678a310a974ad7a229a5737942ca242740 Revert "feat:add team page" -- patch contents already upstream
Successfully rebased and updated refs/heads/ft/home-page-redesign.

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/home-page-redesign)
$ git log
commit d50a51c50a1a0408303be76a29ae80325eb6066d (HEAD -> ft/home-page-redesign)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 14:27:36 2022 +0200

    feat:add faq page

commit 9ddc049a649b34b19ea36b8e20471d673432dbb0
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 14:20:25 2022 +0200

    feat:add contact page

commit ab603fcc41f3c76a73404d59ff49059ce9b608a3 (main)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 15:05:43 2022 +0200

    feat: added home contents

commit 2d855ca9a2b2a0a2a907292ea69f81fa4e5c8530 (origin/main)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 14:56:03 2022 +0200


TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/home-page-redesign)
$

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/home-page-redesign)
$ git add home.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/home-page-redesign)
$ git commit -m "feat: add item lists"
[ft/home-page-redesign 57a85a3] feat: add item lists
 1 file changed, 8 insertions(+)

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/home-page-redesign)
$ git push origin ft/home-page-redesign
fatal: unable to access 'https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git/': Could not resolve host: github.com

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/home-page-redesign)
$ git push origin ft/home-page-redesign
fatal: unable to access 'https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git/': Could not resolve host: github.com

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/home-page-redesign)
$ git pull
fatal: unable to access 'https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git/': Could not resolve host: github.com

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/home-page-redesign)
$ git push origin ft/home-page-redesign
Enumerating objects: 18, done.
Counting objects: 100% (18/18), done.
Delta compression using up to 4 threads
Compressing objects: 100% (15/15), done.
Writing objects: 100% (15/15), 3.75 KiB | 1.25 MiB/s, done.
Total 15 (delta 7), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (7/7), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote:
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
```

### Bundle 4

### Exercise 1

```bash
TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git checkout main
Already on 'main'
M       README.md
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git remote add git-copy https://github.com/Lily-Lilian/Gym-Git-Exercise-2.git

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git remote
git-copy
origin

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git add home.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git commit -m "feat:add home paragraph"
[main 130df91] feat:add home paragraph
 1 file changed, 1 insertion(+)

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git push origin
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 343 bytes | 343.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git
   e06e7d8..130df91  main -> main

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git push git-copy
Enumerating objects: 48, done.
Counting objects: 100% (48/48), done.
Delta compression using up to 4 threads
Compressing objects: 100% (45/45), done.
Writing objects: 100% (48/48), 10.96 KiB | 1020.00 KiB/s, done.
Total 48 (delta 18), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (18/18), done.
To https://github.com/Lily-Lilian/Gym-Git-Exercise-2.git
 * [new branch]      main -> main

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$
```

### Exercise 2

```bash

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/footer)
$ git add footer.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/footer)
$ git commit -m "feat:add footer"
[ft/footer 39e6f17] feat:add footer
 1 file changed, 12 insertions(+)
 create mode 100644 footer.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/footer)
$ git status
On branch ft/footer
nothing to commit, working tree clean

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/footer)
$ git status
On branch ft/footer
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   footer.html

no changes added to commit (use "git add" and/or "git commit -a")

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/footer)
$ git add --all

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/footer)
$ git commit -m "feat:added footer contents"
[ft/footer 3ee64f1] feat:added footer contents
 1 file changed, 4 insertions(+)

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/footer)
$ git push origin ft/footer
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 771 bytes | 771.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions/pull/new/ft/footer
remote:
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/footer -> ft/footer

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/footer)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/squashing)
$ git merge --squash ft/footer
Updating 5662a98..3ee64f1
Fast-forward
Squash commit -- not updating HEAD
 footer.html | 16 ++++++++++++++++
 1 file changed, 16 insertions(+)
 create mode 100644 footer.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/squashing)
$ git log
commit 5662a98d03034c8c56560a2667a6553d11ba3a4b (HEAD -> ft/squashing, origin/main, main)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Wed Oct 26 08:59:58 2022 +0200

    bundle 4

commit 130df9137766e624d941faf4a871989886c11a34 (git-copy/main)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Wed Oct 26 08:50:48 2022 +0200

    feat:add home paragraph

commit e06e7d8102c6962bfa92d2c118434113e81c81cd
Merge: 4594a09 59c83ed
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 15:57:01 2022 +0200

    Merge branch 'main' of https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions

commit 4594a097704b966ef92c853f5ad77d2d4866fd38
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 15:46:34 2022 +0200

    bundle 3 exercise 2

commit ab603fcc41f3c76a73404d59ff49059ce9b608a3
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 15:05:43 2022 +0200

    feat: added home contents

commit 59c83ed25ac00e057bef7638200398d9f32f5dbf
Author: Liliane Iradukunda <98592737+Lily-Lilian@users.noreply.github.com>
Date:   Tue Oct 25 15:02:09 2022 +0200

    Delete team.html

commit 2d855ca9a2b2a0a2a907292ea69f81fa4e5c8530
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 14:56:03 2022 +0200

    bundle 3

commit a61af8cfa3654b0cf315448359b07c99ac45302c
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 13:44:59 2022 +0200

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/squashing)
$ git status
On branch ft/squashing
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   footer.html


TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/squashing)
$ git commit -m "footer changes squashing"
[ft/squashing 82b3889] footer changes squashing
 1 file changed, 16 insertions(+)
 create mode 100644 footer.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/squashing)
$ git log
commit 82b3889291d700d9391636ab8184165c853320e5 (HEAD -> ft/squashing)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Wed Oct 26 09:59:30 2022 +0200

    footer changes squashing

commit 5662a98d03034c8c56560a2667a6553d11ba3a4b (origin/main, main)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Wed Oct 26 08:59:58 2022 +0200

    bundle 4

commit 130df9137766e624d941faf4a871989886c11a34 (git-copy/main)
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Wed Oct 26 08:50:48 2022 +0200

    feat:add home paragraph

commit e06e7d8102c6962bfa92d2c118434113e81c81cd
Merge: 4594a09 59c83ed
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 15:57:01 2022 +0200

    Merge branch 'main' of https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions

commit 4594a097704b966ef92c853f5ad77d2d4866fd38
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 15:46:34 2022 +0200

    bundle 3 exercise 2

commit ab603fcc41f3c76a73404d59ff49059ce9b608a3
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 15:05:43 2022 +0200

    feat: added home contents

commit 59c83ed25ac00e057bef7638200398d9f32f5dbf
Author: Liliane Iradukunda <98592737+Lily-Lilian@users.noreply.github.com>
Date:   Tue Oct 25 15:02:09 2022 +0200

    Delete team.html

commit 2d855ca9a2b2a0a2a907292ea69f81fa4e5c8530
Author: Lily-Lilian <lialsina03@gmail.com>
Date:   Tue Oct 25 14:56:03 2022 +0200


TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/squashing)
$ git checkout ft/footer
Switched to branch 'ft/footer'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/footer)
$ git diff ft/squashing

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/footer)
$ git checkout ft/squashing
Switched to branch 'ft/squashing'

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (ft/squashing)
$ git push origin ft/squashing
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 503 bytes | 503.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions/pull/new/ft/squashing
remote:
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/squashing -> ft/squashing
```

### Bundle 5

### Exercise 1

```bash
TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git pull
Already up to date.

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git add index.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   index.html

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    home.html


TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git commit -m "feat:rename home to index.html"
[main 514d28e] feat:rename home to index.html
 1 file changed, 14 insertions(+)
 create mode 100644 index.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/Desktop/The Gym/Git-Exercise (main)
$ git push origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 247 bytes | 247.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Lily-Lilian/Gym-Git-Exercise-Solutions.git
   c91338b..514d28e  main -> main

```

## Exercise 2

```bash
TheGym@DESKTOP-S5S4V35 MINGW64 ~
$ git clone https://github.com/Lily-Lilian/git-cafe-exercise.git
Cloning into 'git-cafe-exercise'...
remote: Enumerating objects: 107, done.
remote: Counting objects: 100% (107/107), done.
remote: Compressing objects: 100% (101/101), done.
remote: Total 107 (delta 5), reused 104 (delta 4), pack-reused 0
Receiving objects: 100% (107/107), 1.95 MiB | 1.69 MiB/s, done.
Resolving deltas: 100% (5/5), done.

TheGym@DESKTOP-S5S4V35 MINGW64 ~
$ cd git-cafe-exercise

TheGym@DESKTOP-S5S4V35 MINGW64 ~/git-cafe-exercise (main)
$ git add index.html

TheGym@DESKTOP-S5S4V35 MINGW64 ~/git-cafe-exercise (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   index.html


TheGym@DESKTOP-S5S4V35 MINGW64 ~/git-cafe-exercise (main)
$ git commit -m "feat:rename the main title"
[main 10fedb0] feat:rename the main title
 1 file changed, 1 insertion(+), 1 deletion(-)

TheGym@DESKTOP-S5S4V35 MINGW64 ~/git-cafe-exercise (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 345 bytes | 345.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Lily-Lilian/git-cafe-exercise.git
   d1d3f9c..10fedb0  main -> main
```
