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
ad512f0 (HEAD -> main, origin/main, origin/HEAD) readme
pick c1af03b unwanted commits
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
$ git rebase HEAD~3
error: cannot rebase: You have unstaged changes.
error: Please commit or stash them.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git add .

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git commit -m"readme updates"
[main 932f39c] readme updates
 1 file changed, 11 insertions(+)

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git rebase HEAD~3
Current branch main is up to date.
bee8c99 Initial commit

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git rebase HEAD~3
error: cannot rebase: You have unstaged changes.
error: Please commit or stash them.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git add .

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git commit -m"readme updates"
[main 932f39c] readme updates
 1 file changed, 11 insertions(+)

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git rebase HEAD~3
Current branch main is up to date.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git rebase -i
Successfully rebased and updated refs/heads/main.

UMWIZERWA@DESKTOP-6D0H2BN MINGW64 /c/TheGym/Git_advanced_Exercise (main)
$ git rebase -i HEAD~3
Successfully rebased and updated refs/heads/main.

```
</details>
