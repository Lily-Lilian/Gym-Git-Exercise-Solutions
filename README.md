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
