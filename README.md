# Git_advanced_Exercise
<details>
<summary>Part1 - Excercise 1</summary>

Learning Github
```bash
# # Part1  
# challenge 1
PS C:\TheGym\Github\Git_advanced_Exercise> git add .
PS C:\TheGym\Github\Git_advanced_Exercise> git commit -m "chore: Create initial file"
 3 files changed, 0 insertions(+), 0 deletions(-)
 delete mode 100644 test2.md
 delete mode 100644 test3.md
 delete mode 100644 test4.md
PS C:\TheGym\Github\Git_advanced_Exercise> git add .
PS C:\TheGym\Github\Git_advanced_Exercise>  git commit -m "chore: Create another file"
[main 238249a] chore: Create another file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test2.md
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test3.md

nothing added to commit but untracked files present (use "git add" to track)
PS C:\TheGym\Github\Git_advanced_Exercise> git add .
PS C:\TheGym\Github\Git_advanced_Exercise> git commit -m "chore: Create third and fourth files"
[main a454f1a] chore: Create third and fourth files
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md
PS C:\TheGym\Github\Git_advanced_Exercise> git status
PS C:\TheGym\Github\Git_advanced_Exercise> git status
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\TheGym\Github\Git_advanced_Exercise> git log
PS C:\TheGym\Github\Git_advanced_Exercise> git status
On branch main
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\TheGym\Github\Git_advanced_Exercise> ^C
PS C:\TheGym\Github\Git_advanced_Exercise> git status
On branch main
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test4.md

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\TheGym\Github\Git_advanced_Exercise> git log
Author: Umwizer <ruthumwizerwa@gmail.com>

    chore: Create third and fourth files

commit 238249a97c38793862d58f9cbe271b1bc8a467a1
Author: Umwizer <ruthumwizerwa@gmail.com>
Date:   Fri Feb 28 09:46:35 2025 +0200

PS C:\TheGym\Github\Git_advanced_Exercise> git branch
* main
PS C:\TheGym\Github\Git_advanced_Exercise> git log main
Author: Umwizer <ruthumwizerwa@gmail.com>
Date:   Fri Feb 28 09:47:15 2025 +0200

    chore: Create third and fourth files

Author: Umwizer <ruthumwizerwa@gmail.com>
Date:   Fri Feb 28 09:46:35 2025 +0200

PS C:\TheGym\Github\Git_advanced_Exercise> git log --oneline
a454f1a (HEAD -> main) chore: Create third and fourth files
238249a chore: Create another file
6ddd53d chore: Create initial file
1174f13 chore:created four intitial files
bee8c99 (origin/main, origin/HEAD) Initial commit
PS C:\TheGym\Github\Git_advanced_Exercise> git status
On branch main
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

  (use "git add <file>..." to update what will be committed)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test4.md
no changes added to commit (use "git add" and/or "git commit -a")
PS C:\TheGym\Github\Git_advanced_Exercise> git add .
warning: in the working copy of 'test4.md', CRLF will be replaced by LF the next time Git touches it
PS C:\TheGym\Github\Git_advanced_Exercise> git commit --amend -m "add the fourth file to my commit"
[main 1454a1a] add the fourth file to my commit
 Date: Fri Feb 28 09:47:15 2025 +0200
 3 files changed, 36 insertions(+), 2 deletions(-)
 create mode 100644 test3.md
 create mode 100644 test4.md
PS C:\TheGym\Github\Git_advanced_Exercise> git log --oneline
1454a1a (HEAD -> main) add the fourth file to my commit
238249a chore: Create another file
6ddd53d chore: Create initial file
1174f13 chore:created four intitial files
bee8c99 (origin/main, origin/HEAD) Initial commit
PS C:\TheGym\Github\Git_advanced_Exercise> 
PS C:\TheGym\Github\Git_advanced_Exercise> git status
On branch main
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

  (use "git add <file>..." to update what will be committed)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test4.md
no changes added to commit (use "git add" and/or "git commit -a")
PS C:\TheGym\Github\Git_advanced_Exercise> git add .
warning: in the working copy of 'test4.md', CRLF will be replaced by LF the next time Git touches it
PS C:\TheGym\Github\Git_advanced_Exercise> git commit --amend -m "add the fourth file to my commit"
[main 1454a1a] add the fourth file to my commit

```
</details>

<details>
<summary> Part 1 Exercise 2</summary>

```bash
# challenge 2
PS C:\TheGym\Github\Git_advanced_Exercise> git rebase -i HEAD~2
error: cannot rebase: You have unstaged changes.
PS C:\TheGym\Github\Git_advanced_Exercise> git rebase -i HEAD~2
error: cannot rebase: You have unstaged changes.
PS C:\TheGym\Github\Git_advanced_Exercise> git log --oneline   
238249a chore: Create another file
6ddd53d chore: Create initial file
bee8c99 (origin/main, origin/HEAD) Initial commit
error: cannot rebase: You have unstaged changes.
PS C:\TheGym\Github\Git_advanced_Exercise> git add .
warning: in the working copy of 'test4.md', CRLF will be replaced by LF the next time Git touches it
PS C:\TheGym\Github\Git_advanced_Exercise> git commit -m "readme"
[main 2e7a025] readme
 1 file changed, 99 insertions(+), 2 deletions(-)
PS C:\TheGym\Github\Git_advanced_Exercise> git rebase -i HEAD~2  
reword 238249a chore: Create second  file

PS C:\TheGym\Github\Git_advanced_Exercise> git rebase -i HEAD~2
Successfully rebased and updated refs/heads/main.
PS C:\TheGym\Github\Git_advanced_Exercise> git log --oneline     
2e7a025 (HEAD -> main) readme
1454a1a add the fourth file to my commit
238249a chore: Create another file
6ddd53d chore: Create initial file
1174f13 chore:created four intitial files
PS C:\TheGym\Github\Git_advanced_Exercise> git rebase -i HEAD~3  
You can amend the commit now, with

  git commit --amend

Once you are satisfied with your changes, run

reword 238249a chore: Create another file

PS C:\TheGym\Github\Git_advanced_Exercise> git rebase --continue
Successfully rebased and updated refs/heads/main.
PS C:\TheGym\Github\Git_advanced_Exercise> git log --oneline    
2e7a025 (HEAD -> main) readme
1454a1a add the fourth file to my commit
238249a chore: Create another file
6ddd53d chore: Create initial file
1174f13 chore:created four intitial files
PS C:\TheGym\Github\Git_advanced_Exercise> git rebase -i HEAD~3 
Aborting commit due to empty commit message.
You can amend the commit now, with

  git commit --amend

Once you are satisfied with your changes, run

  git rebase --continue
reword 238249a chore: Create another file
chore: Create second  file
I wonder if you are in the middle of another rebase.  If that is the
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
valuable there.
PS C:\TheGym\Github\Git_advanced_Exercise> git rebase --abort  
PS C:\TheGym\Github\Git_advanced_Exercise> git rebase -i HEAD~3
[detached HEAD df85a7e] chore: Create second  file
 Date: Fri Feb 28 09:46:35 2025 +0200
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test2.md
Successfully rebased and updated refs/heads/main.
PS C:\TheGym\Github\Git_advanced_Exercise> git rebase --continue
fatal: no rebase in progress
PS C:\TheGym\Github\Git_advanced_Exercise> git log --oneline    
f8f1971 (HEAD -> main) readme
60dac2c add the fourth file to my commit
df85a7e chore: Create second  file
6ddd53d chore: Create initial file
1174f13 chore:created four intitial files
bee8c99 (origin/main, origin/HEAD) Initial commit
```
</details>

<details>
<summary>Part 1 Challenge 3</summary>

```bash
#challenge 3

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git log --oneline
f8f1971 (HEAD -> main) readme
60dac2c add the fourth file to my commit
df85a7e chore: Create second  file
6ddd53d chore: Create initial file
1174f13 chore:created four intitial files
bee8c99 (origin/main, origin/HEAD) Initial commit

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git rebase -i HEAD~3
error: cannot rebase: You have unstaged changes.
error: Please commit or stash them.
pick 6ddd53d chore: Create initial file
# This is a combination of 2 commits.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git add .

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git commit -m "modified"
[main 8ecb0ca] modified
 1 file changed, 91 insertions(+)

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git rebase -i HEAD~3
Successfully rebased and updated refs/heads/main.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git rebase -i HEAD~4
Successfully rebased and updated refs/heads/main.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git rebase -i HEAD~5
Successfully rebased and updated refs/heads/main.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git rebase -i HEAD~5
[detached HEAD a70f52e] chore: Combination of initial commit and second commit
 Date: Fri Feb 28 09:46:13 2025 +0200
 2 files changed, 0 insertions(+), 0 deletions(-)
 delete mode 100644 test3.md
 delete mode 100644 test4.md
Successfully rebased and updated refs/heads/main.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git log --oneline
6f81312 (HEAD -> main) modified
61d4677 readme
a4a7b50 add the fourth file to my commit
a70f52e chore: Combination of initial commit and second commit
1174f13 chore:created four intitial files
bee8c99 (origin/main, origin/HEAD) Initial commit

```
</details>
<details>
<summary>Part 1 Challenge 4 </summary>

```bash
# # Part1  
# challenge 4
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git log --oneline
9a9f114 (HEAD -> main) changes
a4a7b50 add the fourth file to my commit
a70f52e chore: Combination of initial commit and second commit
1174f13 chore:created four intitial files
bee8c99 (origin/main, origin/HEAD) Initial commit

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git reset --soft a4a7b50

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git branch
* main

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   test4.md

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
        modified:   test4.md


UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git reset HEAD test4.md README.md
Unstaged changes after reset:
M       README.md
M       test4.md

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
        modified:   test4.md

no changes added to commit (use "git add" and/or "git commit -a")
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git add test4.md

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git commit -m "Create Fourth File"
[main 05b2f59] Create Fourth File
 1 file changed, 36 deletions(-)

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git add README.md
warning: in the working copy of 'README.md', CRLF will be replaced by LF the next time Git touches it

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git commit -m "Update README"
[main 157947a] Update README
 1 file changed, 293 insertions(+)

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ ^C

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git add test4.md

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git commit -m "Create Fourth File"
[main 05b2f59] Create Fourth File
 1 file changed, 36 deletions(-)

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git add README.md
warning: in the working copy of 'README.md', CRLF will be replaced by LF the next time Git touches it

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git commit -m "Update README"
[main 157947a] Update README
 1 file changed, 293 insertions(+)


UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git commit -m "Update README"
[main 157947a] Update README
 1 file changed, 293 insertions(+)

 1 file changed, 293 insertions(+)


UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git log --oneline --graph --decorate --all
* 157947a (HEAD -> main) Update README
* 05b2f59 Create Fourth File
* a4a7b50 add the fourth file to my commit
* a70f52e chore: Combination of initial commit and second commit
* 1174f13 chore:created four intitial files
* bee8c99 (origin/main, origin/HEAD) Initial commit
$ git push origin main --force
Enumerating objects: 15, done.
Counting objects: 100% (15/15), done.  
Delta compression using up to 4 threads
Compressing objects: 100% (11/11), done.
Writing objects: 100% (13/13), 2.83 KiB | 362.00 KiB/s, done.
Total 13 (delta 5), reused 5 (delta 1), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (5/5), done.
To https://github.com/Umwizer/Git_advanced_Exercise.git
   bee8c99..157947a  main -> main

```
</details>
<details>
```bash
<summary>Part 1 challenge 5</summary>

</details>