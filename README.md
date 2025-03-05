# Git_advanced_Exercise
# PART 1
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
<summary>Part 1 challenge 5</summary>

```bash

#part 1
## challenge 5
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git commit -m "Cretae Third File "
[main 32cc82f] Cretae Third File
 1 file changed, 124 insertions(+), 1 deletion(-)

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.01 KiB | 207.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Umwizer/Git_advanced_Exercise.git
   157947a..32cc82f  main -> main
pick 05b2f59 Create Fourth File

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git log --oneline
32cc82f (HEAD -> main, origin/main, origin/HEAD) Cretae Third File
157947a Update README
05b2f59 Create Fourth File
a4a7b50 add the fourth file to my commit
a70f52e chore: Combination of initial commit and second commit
1174f13 chore:created four intitial files
bee8c99 Initial commit

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git rebase -i HEAD~2
Successfully rebased and updated refs/heads/main.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git rebase -i HEAD~3
$ git rebase -i HEAD~2
Successfully rebased and updated refs/heads/main.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git rebase -i HEAD~3

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git rebase -i HEAD~3
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git rebase -i HEAD~3
$ git rebase -i HEAD~3
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply 32cc82f... Cretae Third File
error: could not apply 32cc82f... Cretae Third File
hint: Resolve all conflicts manually, mark them as resolved with
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".
hint: Disable this message with "git config advice.mergeConflict false"
Could not apply 32cc82f... Cretae Third File

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main|REBASE 2/3)
Cretae Third File
$ rebase --continue
rebase: unknown option -- continue
usage: rebase [-b BaseAddress] [-o Offset] [-48dOsvV] [-T [FileList | -]] Files...
       rebase -i [-48MOs] [-T [FileList | -]] Files...
       rebase --help or --usage for full help text

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main|REBASE 2/3)
$ git rebase --continue
[detached HEAD 1fb9077] Cretae Third File
 1 file changed, 293 insertions(+)
interactive rebase in progress; onto a4a7b50
Last commands done (3 commands done):
   pick 32cc82f Cretae Third File
   pick 157947a Update README
  (see more in file .git/rebase-merge/done)
No commands remaining.
You are currently rebasing branch 'main' on 'a4a7b50'.
  (all conflicts fixed: run "git rebase --continue")

nothing to commit, working tree clean
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git rebase --skip'
Could not apply 157947a... Update README

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main|REBASE 3/3)
$ git log --oneline
655a41f (HEAD -> main) Merge branch 'main' of https://github.com/Umwizer/Git_advanced_Exercise
1fb9077 Cretae Third File
32cc82f (origin/main, origin/HEAD) Cretae Third File
157947a Update README
05b2f59 Create Fourth File
a4a7b50 add the fourth file to my commit
a70f52e chore: Combination of initial commit and second commit
1174f13 chore:created four intitial files

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git log --oneline
655a41f (HEAD -> main, origin/main, origin/HEAD) Merge branch 'main' of https://github.com/Umwizer/Git_advanced_Exercise
1fb9077 Cretae Third File
32cc82f Cretae Third File
157947a Update README
05b2f59 Create Fourth File
a4a7b50 add the fourth file to my commit
a70f52e chore: Combination of initial commit and second commit
1174f13 chore:created four intitial files

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git rebase -i HEAD~3
error: cannot rebase: You have unstaged changes.
error: Please commit or stash them.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git rebase -i HEAD~4
error: cannot rebase: You have unstaged changes.
error: Please commit or stash them.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git add README.md
pick 05b2f59 Create Fourth File
# This is a combination of 2 commits.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git commit -m 'Add readme.md'
[main 5835f28] Add readme.md
 1 file changed, 7 deletions(-)

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git rebase -i HEAD~4
[detached HEAD f3d0b55] Combine third and Fourth File
 Date: Mon Mar 3 10:35:58 2025 +0200
 2 files changed, 293 insertions(+), 36 deletions(-)
interactive rebase in progress; onto a4a7b50
Last commands done (3 commands done):
   squash 1fb9077 Cretae Third File
   pick 157947a Update README
  (see more in file .git/rebase-merge/done)
Next commands to do (2 remaining commands):
   pick 32cc82f Cretae Third File
   pick 5835f28 Add readme.md
  (use "git rebase --edit-todo" to view and edit)
You are currently rebasing branch 'main' on 'a4a7b50'.
  (all conflicts fixed: run "git rebase --continue")

nothing to commit, working tree clean
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git rebase --skip'
Could not apply 157947a... Update README

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main|REBASE 3/5)
$ git rebase --continue
interactive rebase in progress; onto a4a7b50
Last commands done (5 commands done):
   pick 32cc82f Cretae Third File
   pick 5835f28 Add readme.md
  (see more in file .git/rebase-merge/done)
No commands remaining.
You are currently rebasing branch 'main' on 'a4a7b50'.
  (all conflicts fixed: run "git rebase --continue")

nothing to commit, working tree clean
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git rebase --skip'
Could not apply 5835f28... Add readme.md

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main|REBASE 5/5)
$ git log --oneline
0d67f9a (HEAD) Cretae Third File
f3d0b55 Combine third and Fourth File
a4a7b50 add the fourth file to my commit
a70f52e chore: Combination of initial commit and second commit
1174f13 chore:created four intitial files
bee8c99 Initial commit

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main|REBASE 5/5)
$ git rebase -i HEAD~4
fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something
valuable there.


UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main|REBASE 5/5)
$ git rebase -i HEAD~3
fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something
valuable there.
squash  0d67f9a Cretae Third File
Combine third and Fourth File


UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main|REBASE 5/5)
$ git rebase --continue
Successfully rebased and updated refs/heads/main.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git rebase -i HEAD~3
[detached HEAD b503285] Combine third and Fourth File
 Date: Mon Mar 3 10:35:58 2025 +0200
 2 files changed, 416 insertions(+), 36 deletions(-)
Successfully rebased and updated refs/heads/main.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Github/Git_advanced_Exercise (main)
$ git log --oneline
b503285 (HEAD -> main) Combine third and Fourth File
a4a7b50 add the fourth file to my commit
a70f52e chore: Combination of initial commit and second commit
1174f13 chore:created four intitial files
bee8c99 Initial commit
```
</details>
<details>
<summary>Part1 Challenge  6</summary>

```bash
#part 1
## challenge 6
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git add .
warning: in the working copy of 'unwanted.txt', CRLF will be replaced by LF the next time Git touches it

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git commit -m "unwanted files"
[main 8ad555e] unwanted files   
 1 file changed, 1 insertion(+) 
 create mode 100644 unwanted.txt

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ 
```
</details>
<details>
<summary>Part 1 Challenge7</summary>

```bash

#Part 1
##Challenge 7
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git log --oneline
4c6452f (HEAD -> main) rebasing
7eae152 readme updates
069ddc1 unwanted commits
4ead034 Cretae Third File
58edd1c unwanted files
1fb9077 Cretae Third File
05b2f59 Create Fourth File
a4a7b50 add the fourth file to my commit
a70f52e chore: Combination of initial commit and second commit
1174f13 chore:created four intitial files
bee8c99 Initial commit

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git rebase -i HEAD~5
Successfully rebased and updated refs/heads/main.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git log --oneline
78df94d (HEAD -> main) unwanted files
beb2d0a rebasing
4da9da9 readme updates
66743cb unwanted commits
25a0e88 Cretae Third File
1fb9077 Cretae Third File
05b2f59 Create Fourth File
a4a7b50 add the fourth file to my commit
a70f52e chore: Combination of initial commit and second commit
1174f13 chore:created four intitial files
bee8c99 Initial commit
```
</details>
<details>
<summary>Part 1 Challenge 8</summary>

```bash
# part 1 
## challenge 8
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/branch)
$ git add test5.md

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/branch)
$ git commit -m "Implemented Test 5"
[ft/branch 31e92dd] Implemented Test 5
 1 file changed, 1 insertion(+)       
 create mode 100644 test5.md

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/branch)
$ git log --oneline
31e92dd (HEAD -> ft/branch) Implemented Test 5
31e92dd (HEAD -> ft/branch) Implemented Test 5
25a87d8 (origin/main, origin/HEAD, main) challenge 7
f45f6e2 rebasing
ae26d1e readme updates
ad512f0 readme
c1af03b unwanted commits
d4b463f unwanted files
655a41f Merge branch 'main' of https://github.com/Umwizer/Git_advanced_Exercise
1fb9077 Cretae Third File
32cc82f Cretae Third File
157947a Update README
05b2f59 Create Fourth File
a4a7b50 add the fourth file to my commit
a70f52e chore: Combination of initial commit and second commit
1174f13 chore:created four intitial files
bee8c99 Initial commit
...skipping...

                   SUMMARY OF LESS COMMANDS

      Commands marked with * may be preceded by a number, N.
      Notes in parentheses indicate the behavior if N is given.
      A key preceded by a caret indicates the Ctrl key; thus ^K is ctrl-K.

  h  H                 Display this help.
  q  :q  Q  :Q  ZZ     Exit.
 ---------------------------------------------------------------------------

                           MOVING

  e  ^E  j  ^N  CR  *  Forward  one line   (or N lines).
  y  ^Y  k  ^K  ^P  *  Backward one line   (or N lines).
HELP -- Press RETURN for more, or q when done...skipping...
25a87d8 (origin/main, origin/HEAD, main) challenge 7
f45f6e2 rebasing
ae26d1e readme updates
ad512f0 readme
c1af03b unwanted commits
d4b463f unwanted files
655a41f Merge branch 'main' of https://github.com/Umwizer/Git_advanced_Exercise
1fb9077 Cretae Third File
32cc82f Cretae Third File
157947a Update README
05b2f59 Create Fourth File
a4a7b50 add the fourth file to my commit
a70f52e chore: Combination of initial commit and second commit
1174f13 chore:created four intitial files
bee8c99 Initial commit
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git cherry-pick 31e92dd
[main 5f556e0] Implemented Test 5
 Date: Tue Mar 4 12:13:11 2025 +0200
 1 file changed, 1 insertion(+)
 create mode 100644 test5.md

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git log --oneline
5f556e0 (HEAD -> main) Implemented Test 5
25a87d8 (origin/main, origin/HEAD) challenge 7
f45f6e2 rebasing
ae26d1e readme updates
ad512f0 readme
c1af03b unwanted commits
d4b463f unwanted files
655a41f Merge branch 'main' of https://github.com/Umwizer/Git_advanced_Exercise
1fb9077 Cretae Third File
32cc82f Cretae Third File
157947a Update README
05b2f59 Create Fourth File
a4a7b50 add the fourth file to my commit
a70f52e chore: Combination of initial commit and second commit
1174f13 chore:created four intitial files

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 280 bytes | 280.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Umwizer/Git_advanced_Exercise.git
   25a87d8..5f556e0  main -> main
```
</details>

<details>
<summary>Part 1  Challenge 9</summary>

```bash
# part 1 Challenge 9
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git log --oneline --graph --decorate --all
* 88ad43b (HEAD -> main, origin/main, origin/HEAD) Updating ReadMe
* 521f04b challenge 8
* 4e958f0 updated readme
* 5f556e0 Implemented Test 5
| * 31e92dd (ft/branch) Implemented Test 5
|/
* 25a87d8 challenge 7
* f45f6e2 rebasing
* ae26d1e readme updates
* ad512f0 readme
* c1af03b unwanted commits
* d4b463f unwanted files
*   655a41f Merge branch 'main' of https://github.com/Umwizer/Git_advanced_Exercise
|\
| * 32cc82f Cretae Third File
| * 157947a Update README
* | 1fb9077 Cretae Third File
|/
* 05b2f59 Create Fourth File
* a4a7b50 add the fourth file to my commit
* a70f52e chore: Combination of initial commit and second commit
* 1174f13 chore:created four intitial files
* bee8c99 Initial commit

```

</details>

<details>
<summary>Part1 Challenge 10 </summary>

```bash
#part 1 challenge 10
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git reflog
88ad43b (HEAD -> main, origin/main, origin/HEAD) HEAD@{0}: commit: Updating ReadMe
521f04b HEAD@{1}: commit: challenge 8
4e958f0 HEAD@{2}: commit: updated readme
5f556e0 HEAD@{3}: cherry-pick: Implemented Test 5
25a87d8 HEAD@{4}: checkout: moving from main to main
25a87d8 HEAD@{5}: checkout: moving from ft/branch to main
31e92dd (ft/branch) HEAD@{6}: checkout: moving from main to ft/branch      
25a87d8 HEAD@{7}: reset: moving to 25a87d8ee13fe22e2c675b3ff5c5af67adaf50ee
25a87d8 HEAD@{8}: checkout: moving from ft/branch to main
31e92dd (ft/branch) HEAD@{9}: commit: Implemented Test 5
25a87d8 HEAD@{10}: checkout: moving from main to ft/branch
25a87d8 HEAD@{11}: pull origin main --rebase (finish): returning to refs/heads/main
25a87d8 HEAD@{12}: pull origin main --rebase (pick): challenge 7
f45f6e2 HEAD@{13}: pull origin main --rebase (pick): rebasing
ae26d1e HEAD@{14}: pull origin main --rebase (pick): readme updates
ad512f0 HEAD@{15}: pull origin main --rebase (start): checkout ad512f0b54ec6b6d00e62a1815c1c3c1c7ffc56d
8d11aa7 HEAD@{16}: commit: challenge 7
5f556e0 HEAD@{3}: cherry-pick: Implemented Test 5
25a87d8 HEAD@{4}: checkout: moving from main to main
25a87d8 HEAD@{5}: checkout: moving from ft/branch to main
31e92dd (ft/branch) HEAD@{6}: checkout: moving from main to ft/branch
25a87d8 HEAD@{7}: reset: moving to 25a87d8ee13fe22e2c675b3ff5c5af67adaf50ee
25a87d8 HEAD@{8}: checkout: moving from ft/branch to main
31e92dd (ft/branch) HEAD@{9}: commit: Implemented Test 5
25a87d8 HEAD@{10}: checkout: moving from main to ft/branch
25a87d8 HEAD@{11}: pull origin main --rebase (finish): returning to refs/heads/main
25a87d8 HEAD@{12}: pull origin main --rebase (pick): challenge 7
f45f6e2 HEAD@{13}: pull origin main --rebase (pick): rebasing
ae26d1e HEAD@{14}: pull origin main --rebase (pick): readme updates
ad512f0 HEAD@{15}: pull origin main --rebase (start): checkout ad512f0b54ec6b6d00e62a1815c1c3c1c7ffc56d
8d11aa7 HEAD@{16}: commit: challenge 7
25a87d8 HEAD@{7}: reset: moving to 25a87d8ee13fe22e2c675b3ff5c5af67adaf50ee
25a87d8 HEAD@{8}: checkout: moving from ft/branch to main
31e92dd (ft/branch) HEAD@{9}: commit: Implemented Test 5
25a87d8 HEAD@{10}: checkout: moving from main to ft/branch
25a87d8 HEAD@{11}: pull origin main --rebase (finish): returning to refs/heads/main
25a87d8 HEAD@{12}: pull origin main --rebase (pick): challenge 7
f45f6e2 HEAD@{13}: pull origin main --rebase (pick): rebasing
ae26d1e HEAD@{14}: pull origin main --rebase (pick): readme updates
ad512f0 HEAD@{15}: pull origin main --rebase (start): checkout ad512f0b54ec6b6d00e62a1815c1c3c1c7ffc56d
8d11aa7 HEAD@{16}: commit: challenge 7
25a87d8 HEAD@{8}: checkout: moving from ft/branch to main
31e92dd (ft/branch) HEAD@{9}: commit: Implemented Test 5
25a87d8 HEAD@{10}: checkout: moving from main to ft/branch
25a87d8 HEAD@{11}: pull origin main --rebase (finish): returning to refs/heads/main
25a87d8 HEAD@{12}: pull origin main --rebase (pick): challenge 7
f45f6e2 HEAD@{13}: pull origin main --rebase (pick): rebasing
ae26d1e HEAD@{14}: pull origin main --rebase (pick): readme updates
ad512f0 HEAD@{15}: pull origin main --rebase (start): checkout ad512f0b54ec6b6d00e62a1815c1c3c1c7ffc56d
8d11aa7 HEAD@{16}: commit: challenge 7
25a87d8 HEAD@{10}: checkout: moving from main to ft/branch
25a87d8 HEAD@{11}: pull origin main --rebase (finish): returning to refs/heads/main
25a87d8 HEAD@{12}: pull origin main --rebase (pick): challenge 7
f45f6e2 HEAD@{13}: pull origin main --rebase (pick): rebasing
ae26d1e HEAD@{14}: pull origin main --rebase (pick): readme updates
ad512f0 HEAD@{15}: pull origin main --rebase (start): checkout ad512f0b54ec6b6d00e62a1815c1c3c1c7ffc56d
8d11aa7 HEAD@{16}: commit: challenge 7
25a87d8 HEAD@{12}: pull origin main --rebase (pick): challenge 7
f45f6e2 HEAD@{13}: pull origin main --rebase (pick): rebasing
ae26d1e HEAD@{14}: pull origin main --rebase (pick): readme updates
ad512f0 HEAD@{15}: pull origin main --rebase (start): checkout ad512f0b54ec6b6d00e62a1815c1c3c1c7ffc56d
8d11aa7 HEAD@{16}: commit: challenge 7
ae26d1e HEAD@{14}: pull origin main --rebase (pick): readme updates
ad512f0 HEAD@{15}: pull origin main --rebase (start): checkout ad512f0b54ec6b6d00e62a1815c1c3c1c7ffc56d
8d11aa7 HEAD@{16}: commit: challenge 7
ad512f0 HEAD@{15}: pull origin main --rebase (start): checkout ad512f0b54ec6b6d00e62a1815c1c3c1c7ffc56d
8d11aa7 HEAD@{16}: commit: challenge 7
8d11aa7 HEAD@{16}: commit: challenge 7
78df94d HEAD@{17}: rebase (finish): returning to refs/heads/main
78df94d HEAD@{17}: rebase (finish): returning to refs/heads/main
78df94d HEAD@{18}: rebase (pick): unwanted files
beb2d0a HEAD@{19}: rebase (pick): rebasing
4da9da9 HEAD@{20}: rebase (pick): readme updates
66743cb HEAD@{21}: rebase (pick): unwanted commits
25a0e88 HEAD@{22}: rebase (pick): Cretae Third File
beb2d0a HEAD@{19}: rebase (pick): rebasing
4da9da9 HEAD@{20}: rebase (pick): readme updates
66743cb HEAD@{21}: rebase (pick): unwanted commits
25a0e88 HEAD@{22}: rebase (pick): Cretae Third File
66743cb HEAD@{21}: rebase (pick): unwanted commits
25a0e88 HEAD@{22}: rebase (pick): Cretae Third File
1fb9077 HEAD@{23}: rebase (start): checkout HEAD~5
1fb9077 HEAD@{23}: rebase (start): checkout HEAD~5
4c6452f HEAD@{24}: rebase (abort): returning to refs/heads/main
dde3232 HEAD@{25}: rebase (pick): unwanted files
a1e3222 HEAD@{26}: rebase (pick): Cretae Third File
1fb9077 HEAD@{27}: rebase (start): checkout HEAD~5
4c6452f HEAD@{28}: rebase (finish): returning to refs/heads/main



```
</details>

# PART 2

<details>
<summary>Part2 Challenge 1</summary>

```bash
#Part 1
## Challenge 1  
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git branch ft/new-feature

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git checkout ft/new-feature
Switched to branch 'ft/new-feature'
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git checkout ft/new-feature
Switched to branch 'ft/new-feature'
$ git checkout ft/new-feature
Switched to branch 'ft/new-feature'
Switched to branch 'ft/new-feature'


UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/new-feature)
$ git branch
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/new-feature)
$ git branch
  ft/branch
$ git branch
  ft/branch
  ft/branch
* ft/new-feature
  main

* ft/new-feature
  main

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/new-feature)
  main

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/new-feature)
```
</details>
<details>
<summary>Part 1 Challenge 2</summary>

```bash
#Part 1
## Challenge 3

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/new-feature)
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/new-feature)
$ git add .
$ git add .

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/new-feature)
$ git commit -m "Implemented core functionality for new feature".
[ft/new-feature 29aa610] Implemented core functionality for new feature.
 2 files changed, 21 insertions(+)
 create mode 100644 feature.txt

```
</details>

<details>
<summary>Part2 Challenge 3</summary>

```bash

#part 1
## Challenge 3
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/new-feature)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git add readme.txt

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git commit -m "Added readme.txt with project intro"
[main 93741be] Added readme.txt with project intro
 1 file changed, 1 insertion(+)
 create mode 100644 readme.txt
 ```
 </details>

<details>
<summary>Part 2 Challenge 4 </summary>

```bash
A "local branch" in Git refers to a branch that exists solely on your local machine, while a "remote branch" is a copy of that local branch stored on a remote Git repository like GitHub, allowing you to share your work with others and collaborate on the same codebase; to synchronize changes between your local and remote repositories, you "push" your local branches to the remote repository and "pull" changes from the remote to update your local workspace. 
Key points about local and remote branches:
Local Branches:
Created and managed directly on your computer. 
Only visible to you on your machine. 
Used for active development and making changes to your code. 
Remote Branches:
Copies of your local branches stored on a remote Git server (like GitHub). 
Accessible to other team members who have access to the remote repository. 
Used to share your work, collaborate on projects, and merge changes from other developers. 
How to push and pull branches:
Pushing a local branch to a remote repository:
Command: git push origin <branch-name>
Explanation: This command sends your local branch named <branch-name> to the remote repository called "origin".
Pulling changes from a remote branch to your local repository:
Command: git pull origin <branch-name>
Explanation: This command fetches the latest version of the remote branch named <branch-name> from "origin" and merges it into your local branch. 
Important considerations:
Setting up upstream tracking:
When creating a new local branch, it's often recommended to set up "upstream tracking" to easily push and pull changes to the corresponding remote branch. You can do this by adding the -u flag when you first push your local branch: git push origin <branch-name> -u. 
Managing merge conflicts:
If multiple developers are working on the same remote branch, you may encounter merge conflicts when pulling changes from the remote repository. Git will prompt you to resolve these conflicts manually before you can complete the pull operation. 
```
</details>

<details>
<summary>Part2 Challenge 5 </summary>

```bash

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git pull origin main
From https://github.com/Umwizer/Git_advanced_Exercise
 * branch            main       -> FETCH_HEAD        
Already up to date.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git branch --merged
  ft/new-feature
* main

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git branch -d ft/new-feature
Deleted branch ft/new-feature (was f31f308).

```
</details>
<details>
<summary>Part2  Challenge 6 </summary>

```bash
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git log --oneline
95bc6d3 (HEAD -> main, origin/main, origin/HEAD) Challenge 6
2b3cedb readme data
10044f6 updated readme
2256218 Added readme.txt with project intro
a69ee68 Merge pull request #1 from Umwizer/ft/new-feature   
f31f308 (origin/ft/new-feature) updates to readme.     
29aa610 Implemented core functionality for new feature.
28867a0 readme updating
e68b0a0 challenge 10
88ad43b Updating ReadMe
521f04b challenge 8
4e958f0 updated readme
5f556e0 Implemented Test 5
25a87d8 challenge 7       
f45f6e2 rebasing
ae26d1e readme updates    
ad512f0 readme
c1af03b unwanted commits  
d4b463f unwanted files
521f04b challenge 8
4e958f0 updated readme
5f556e0 Implemented Test 5
25a87d8 challenge 7
f45f6e2 rebasing
ae26d1e readme updates
ad512f0 readme
c1af03b unwanted commits
d4b463f unwanted files
655a41f Merge branch 'main' of https://github.com/Umwizer/Git_advanced_Exercise
1fb9077 Cretae Third File
ad512f0 readme
c1af03b unwanted commits
d4b463f unwanted files
655a41f Merge branch 'main' of https://github.com/Umwizer/Git_advanced_Exercise
1fb9077 Cretae Third File
32cc82f Cretae Third File
157947a Update README
655a41f Merge branch 'main' of https://github.com/Umwizer/Git_advanced_Exercise
1fb9077 Cretae Third File
32cc82f Cretae Third File
157947a Update README
32cc82f Cretae Third File
157947a Update README
05b2f59 Create Fourth File
05b2f59 Create Fourth File
a4a7b50 add the fourth file to my commit
a70f52e chore: Combination of initial commit and second commit
1174f13 chore:created four intitial files
a70f52e chore: Combination of initial commit and second commit
1174f13 chore:created four intitial files

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git checkout -b ft/new-branch-from-commit a4a7b50
Switched to a new branch 'ft/new-branch-from-commit'
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/new-branch-from-commit)
$ git branch
  ft/branch
* ft/new-branch-from-commit
  main
  main

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/new-branch-from-commit)
$ git push origin ft/new-branch-from-commit
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'ft/new-branch-from-commit' on GitHub by visiting:
remote:
remote: Create a pull request for 'ft/new-branch-from-commit' on GitHub by visiting:
remote:      https://github.com/Umwizer/Git_advanced_Exercise/pull/new/ft/new-branch-from-commit
remote:      https://github.com/Umwizer/Git_advanced_Exercise/pull/new/ft/new-branch-from-commit
remote:
To https://github.com/Umwizer/Git_advanced_Exercise.git
remote:
To https://github.com/Umwizer/Git_advanced_Exercise.git
 * [new branch]      ft/new-branch-from-commit -> ft/new-branch-from-commit

 * [new branch]      ft/new-branch-from-commit -> ft/new-branch-from-commit


UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/new-branch-from-commit)
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/new-branch-from-commit)
$ git checkout main
error: Your local changes to the following files would be overwritten by checkout:
        README.md
Please commit your changes or stash them before you switch branches.
Aborting

$ git checkout main
error: Your local changes to the following files would be overwritten by checkout:
        README.md
Please commit your changes or stash them before you switch branches.
Aborting

Please commit your changes or stash them before you switch branches.
Aborting

Aborting


UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/new-branch-from-commit)
$ git add .

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/new-branch-from-commit)
$ git commit -m "challenge 6"
[ft/new-branch-from-commit c0dcd39] challenge 6
 1 file changed, 1180 insertions(+)
 UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/new-branch-from-commit)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
```

</details>

<details>
<summary>Part1 Challenge 7 </summary>

```bash
#part2
## Challenge 7
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/new-branch-from-commit)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git pull origin main
From https://github.com/Umwizer/Git_advanced_Exercise
 * branch            main       -> FETCH_HEAD        
Already up to date.
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git branch
  ft/branch
  ft/new-branch-from-commit
* main

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
* main
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git log --oneline
4d0cd08 (HEAD -> main, origin/main, origin/HEAD) Challenge 6  read me
86bd4fc Challenge 6  read me
95bc6d3 Challenge 6
2b3cedb readme data
10044f6 updated readme
2256218 Added readme.txt with project intro
a69ee68 Merge pull request #1 from Umwizer/ft/new-feature
f31f308 (origin/ft/new-feature) updates to readme.     
29aa610 Implemented core functionality for new feature.
28867a0 readme updating
e68b0a0 challenge 10
88ad43b Updating ReadMe
521f04b challenge 8
4e958f0 updated readme
5f556e0 Implemented Test 5
25a87d8 challenge 7
f45f6e2 rebasing
ae26d1e readme updates
ad512f0 readme
c1af03b unwanted commits
d4b463f unwanted files
655a41f Merge branch 'main' of https://github.com/Umwizer/Git_advanced_Exercise
1fb9077 Cretae Third File
32cc82f Cretae Third File
157947a Update README
05b2f59 Create Fourth File
a4a7b50 (origin/ft/new-branch-from-commit) add the fourth file to my commit
a70f52e chore: Combination of initial commit and second commit
1174f13 chore:created four intitial files
bee8c99 Initial commit
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git merge ft/new-branch-from-commit a4a7b50
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
Automatic merge failed; fix conflicts and then commit the result.
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main|MERGING)
$ git add .

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main|MERGING)
$ git commit -m"Merge feature branch ft/new-branch-from-commit into main"
[main 511b040] Merge feature branch ft/new-branch-from-commit into main

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git push origin main
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 592 bytes | 592.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main|MERGING)
$ git commit -m"Merge feature branch ft/new-branch-from-commit into main"
[main 511b040] Merge feature branch ft/new-branch-from-commit into main

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git push origin main
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 592 bytes | 592.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git push origin main
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 592 bytes | 592.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 592 bytes | 592.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Umwizer/Git_advanced_Exercise.git
   4d0cd08..511b040  main -> main
Writing objects: 100% (4/4), 592 bytes | 592.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Umwizer/Git_advanced_Exercise.git
   4d0cd08..511b040  main -> main
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Umwizer/Git_advanced_Exercise.git
   4d0cd08..511b040  main -> main

```
</details>
<details>
<summary>Part2 Challenge8</summary>

```bash
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git branch
  ft/branch
  ft/new-branch-from-commit
* main

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
* main

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git merge ft/new-branch-from-commit a4a7b50
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
Automatic merge failed; fix conflicts and then commit the result.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main|MERGING)
$ git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main|MERGING)
$ git add .

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main|MERGING)
$ git commit -m"Merge feature branch ft/new-branch-from-commit into main"
[main 511b040] Merge feature branch ft/new-branch-from-commit into main

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git push origin main
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 592 bytes | 592.00 KiB/s, done. 
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)

The most similar command is
        add

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main|MERGING)
$ git add .

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main|MERGING)
$ git commit -m"Merge feature branch ft/new-branch-from-commit into main"
[main 511b040] Merge feature branch ft/new-branch-from-commit into main

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git push origin main
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 592 bytes | 592.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main|MERGING)
$ git commit -m"Merge feature branch ft/new-branch-from-commit into main"
[main 511b040] Merge feature branch ft/new-branch-from-commit into main

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git push origin main
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 592 bytes | 592.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git push origin main
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 592 bytes | 592.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 592 bytes | 592.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Umwizer/Git_advanced_Exercise.git
   4d0cd08..511b040  main -> main
Writing objects: 100% (4/4), 592 bytes | 592.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Umwizer/Git_advanced_Exercise.git
   4d0cd08..511b040  main -> main
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Umwizer/Git_advanced_Exercise.git
   4d0cd08..511b040  main -> main
```
</details>

<details>
<summary>Part2 Challenge9</summary>

```bash
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/new-branch-from-commit)
$ git branch -m ft/new-branch-from-commit ft/improved-branch-name

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (ft/improved-branch-name)

```
</details>
<details>
<summary>Part2 Challenge10</summary>

```bash
#Part 2
##Challenge 10


```bash
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git log --oneline
f31b488 (HEAD -> main, origin/main, origin/ft/new-branch-from-commit, origin/HEAD) Readme Updates
fce13f4 changes in readme Challenge 7
511b040 Merge feature branch ft/new-branch-from-commit into main
4d0cd08 Challenge 6  read me
86bd4fc Challenge 6  read me
c0dcd39 challenge 6
95bc6d3 Challenge 6
2b3cedb readme data
10044f6 updated readme
2256218 Added readme.txt with project intro
a69ee68 Merge pull request #1 from Umwizer/ft/new-feature
f31f308 (origin/ft/new-feature) updates to readme.       
29aa610 Implemented core functionality for new feature.  
28867a0 readme updating
e68b0a0 challenge 10
88ad43b Updating ReadMe
521f04b challenge 8
4e958f0 updated readme
5f556e0 Implemented Test 5
25a87d8 challenge 7
f45f6e2 rebasing
ae26d1e readme updates
ad512f0 readme
c1af03b unwanted commits
d4b463f unwanted files
655a41f Merge branch 'main' of https://github.com/Umwizer/Git_advanced_Exercise
1fb9077 Cretae Third File
32cc82f Cretae Third File
157947a Update README
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git checkout 86bd4fc
Note: switching to '86bd4fc'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 86bd4fc Challenge 6  read me

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise ((86bd4fc...))
$ git checkout main
Previous HEAD position was 86bd4fc Challenge 6  read me
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

```
</details>

# PART 3
<details>
<summary>Part3 Challenge 1 </summary>

```bash
#part 3
## challenge 1
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git stash
Saved working directory and index state WIP on main: 32b7421 readme updates

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git stash list
stash@{0}: WIP on main: 32b7421 readme updates


```
</details>
<details>
<summary>Part3 Challenge 2 </summary>

```bash
#Part 3
## challenge 2
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git stash pop
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   test8.md

Dropped refs/stash@{0} (3ff1341a5bbd26814f914f63437c3426e5ac4cfe)

```
</details>
<details>
<summary>Part3 Challenge3</summary>

```bash
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git checkout -b conflict-branch
Switched to a new branch 'conflict-branch'

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (conflict-branch)
$ git add example.txt

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (conflict-branch)
$ git commit -m"Modify new file in new branch"
[conflict-branch f617c87] Modify new file in new branch
 2 files changed, 2 insertions(+)
 create mode 100644 example.txt
 create mode 100644 test8.md

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (conflict-branch)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git merge conflict-branch
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 772 bytes | 386.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Umwizer/Git_advanced_Exercise.git
   32b7421..7ff4a1d  main -> main
```
</details>
<details>
<summary>Part3 Challenge4</summary>

```bash
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git branch
  conflict-branch
  ft/branch
  ft/improved-branch-name
* main

hii ruth
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git merge  conflict-branch
Auto-merging example.txt
CONFLICT (add/add): Merge conflict in example.txt
Automatic merge failed; fix conflicts and then commit the result.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main|MERGING)
$ git mergetool

This message is displayed because 'merge.tool' is not configured.
See 'git mergetool --tool-help' or 'git help config' for more details.
'git mergetool' will now attempt to use one of the following tools:
opendiff kdiff3 tkdiff xxdiff meld tortoisemerge gvimdiff diffuse diffmerge ecmerge p4merge araxis bc codecompare smerge emerge vimdiff nvimdiff
Merging:
example.txt

Normal merge conflict for 'example.txt':
  {local}: created file
  {remote}: created file
Hit return to start merge resolution tool (vimdiff):
3 files to edit

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main|MERGING)
UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main|MERGING)
$ git add .

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main|MERGING)
$ git commit -m"readme"
[main 6251533] readme

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git push origin main
Enumerating objects: 14, done.
Counting objects: 100% (14/14), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (9/9), 1.64 KiB | 280.00 KiB/s, done.
Total 9 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
To https://github.com/Umwizer/Git_advanced_Exercise.git
   7ff4a1d..6251533  main -> main
```
</details>


<details>
<summary>Part3 Challenge 5</summary>

```bash

```
</details>