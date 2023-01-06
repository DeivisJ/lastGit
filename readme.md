Admin@MIS MINGW64 ~
$ ls
'3D Objects'/
 AppData/
'Application Data'@
 Contacts/
 Cookies@
 Desktop/
 Documents/
 Downloads/
 Favorites/
 IntelGraphicsProfiles/
 Links/
'Local Settings'@
 MicrosoftEdgeBackups/
 Music/
'My Documents'@
 NTUSER.DAT
 NTUSER.DAT{fd9a35db-49fe-11e9-aa2c-248a07783950}.TM.blf
 NTUSER.DAT{fd9a35db-49fe-11e9-aa2c-248a07783950}.TMContainer00000000000000000001.regtrans-ms
 NTUSER.DAT{fd9a35db-49fe-11e9-aa2c-248a07783950}.TMContainer00000000000000000002.regtrans-ms
 NetHood@
 OneDrive/
 Pictures/
 PrintHood@
 Recent@
'Saved Games'/
 Searches/
 SendTo@
'Start Menu'@
 Templates@
 Untitled.ipynb
 Untitled1.ipynb
 Videos/
 eclipse/
 eclipse-workspace/
 ntuser.dat.LOG1
 ntuser.dat.LOG2
 ntuser.ini
 qa/
 seaborn-data/
 source/

Admin@MIS MINGW64 ~
$ cd qa

Admin@MIS MINGW64 ~/qa
$ ls
gitDemo/

Admin@MIS MINGW64 ~/qa
$ mkdir LastGit

Admin@MIS MINGW64 ~/qa
$ cd LastGit

Admin@MIS MINGW64 ~/qa/LastGit
$ echo "# lastGit" >> readme.md

Admin@MIS MINGW64 ~/qa/LastGit
$ git init
Initialized empty Git repository in C:/Users/Admin/qa/LastGit/.git/

Admin@MIS MINGW64 ~/qa/LastGit (master)
$ git add readme.md
warning: in the working copy of 'readme.md', LF will be replaced by CRLF the next time Git touches it

Admin@MIS MINGW64 ~/qa/LastGit (master)
$ git commit -m "first commit"
[master (root-commit) 6aa6338] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 readme.md

Admin@MIS MINGW64 ~/qa/LastGit (master)
$ git branch -M main
git remote add origin https://github.com/DeivisJ/lastGit.git
git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 227 bytes | 227.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/DeivisJ/lastGit.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git push -u origin main
Everything up-to-date
branch 'main' set up to track 'origin/main'.

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ notepad readme.md

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git branch dev

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git checkout dev
Switched to branch 'dev'
M       readme.md

Admin@MIS MINGW64 ~/qa/LastGit (dev)
$ notepad readme.md

Admin@MIS MINGW64 ~/qa/LastGit (dev)
$ git checkout main
Switched to branch 'main'
M       readme.md
Your branch is up to date with 'origin/main'.

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git add readme.md
warning: in the working copy of 'readme.md', LF will be replaced by CRLF the next time Git touches it

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git commit -m "main branch commit"
[main 17402aa] main branch commit
 1 file changed, 5 insertions(+)

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 302 bytes | 302.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/DeivisJ/lastGit.git
   6aa6338..17402aa  main -> main

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git checkout dev
Switched to branch 'dev'

Admin@MIS MINGW64 ~/qa/LastGit (dev)
$ git add readme.md

Admin@MIS MINGW64 ~/qa/LastGit (dev)
$ git commit -m "created dev branch"
On branch dev
nothing to commit, working tree clean

Admin@MIS MINGW64 ~/qa/LastGit (dev)
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Admin@MIS MINGW64 ~/qa/LastGit (dev)
$ git push --set-upstream origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/DeivisJ/lastGit/pull/new/dev
remote:
To https://github.com/DeivisJ/lastGit.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

Admin@MIS MINGW64 ~/qa/LastGit (dev)
$ git log --oneline
6aa6338 (HEAD -> dev, origin/dev) first commit

Admin@MIS MINGW64 ~/qa/LastGit (dev)
$ git reset 6aa6338

Admin@MIS MINGW64 ~/qa/LastGit (dev)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git log --oneline
17402aa (HEAD -> main, origin/main) main branch commit
6aa6338 (origin/dev, dev) first commit

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git reset 17402aa

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git reset --hard 17402aa
HEAD is now at 17402aa main branch commit

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ notepad readme.md

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git add readme.md

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git commit -m "main branch commit"
[main 6c9e972] main branch commit
 1 file changed, 2 deletions(-)

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (1/1), done.
Writing objects: 100% (3/3), 282 bytes | 282.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/DeivisJ/lastGit.git
   17402aa..6c9e972  main -> main

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ notepad readme.md

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git branch dev
fatal: a branch named 'dev' already exists

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git pull
Already up to date.

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git checkout dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

Admin@MIS MINGW64 ~/qa/LastGit (dev)
$ notepad readme.md

Admin@MIS MINGW64 ~/qa/LastGit (dev)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git branch development

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git checkout development
Switched to branch 'development'

Admin@MIS MINGW64 ~/qa/LastGit (development)
$ notepad readme.md

Admin@MIS MINGW64 ~/qa/LastGit (development)
$ git add readme.md

Admin@MIS MINGW64 ~/qa/LastGit (development)
$ git commit -m "dvelopment branch code"
[development 29de78c] dvelopment branch code
 1 file changed, 2 insertions(+)

Admin@MIS MINGW64 ~/qa/LastGit (development)
$ git push
fatal: The current branch development has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin development

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Admin@MIS MINGW64 ~/qa/LastGit (development)
$ git push --set-upstream origin development
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 309 bytes | 309.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'development' on GitHub by visiting:
remote:      https://github.com/DeivisJ/lastGit/pull/new/development
remote:
To https://github.com/DeivisJ/lastGit.git
 * [new branch]      development -> development
branch 'development' set up to track 'origin/development'.

Admin@MIS MINGW64 ~/qa/LastGit (development)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git branch feat1

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git checkout feat1
Switched to branch 'feat1'

Admin@MIS MINGW64 ~/qa/LastGit (feat1)
$ notepad readme.md

Admin@MIS MINGW64 ~/qa/LastGit (feat1)
$ git add readme.md

Admin@MIS MINGW64 ~/qa/LastGit (feat1)
$ git commit -m "Feature 1 branch added"
[feat1 5a9426a] Feature 1 branch added
 1 file changed, 4 insertions(+)

Admin@MIS MINGW64 ~/qa/LastGit (feat1)
$ git ush
git: 'ush' is not a git command. See 'git --help'.

The most similar command is
        push

Admin@MIS MINGW64 ~/qa/LastGit (feat1)
$ git push
fatal: The current branch feat1 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin feat1

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Admin@MIS MINGW64 ~/qa/LastGit (feat1)
$ git push --set-upstream origin feat1
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Writing objects: 100% (3/3), 299 bytes | 299.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'feat1' on GitHub by visiting:
remote:      https://github.com/DeivisJ/lastGit/pull/new/feat1
remote:
To https://github.com/DeivisJ/lastGit.git
 * [new branch]      feat1 -> feat1
branch 'feat1' set up to track 'origin/feat1'.

Admin@MIS MINGW64 ~/qa/LastGit (feat1)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git branch feat2

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git checkout feat2
Switched to branch 'feat2'

Admin@MIS MINGW64 ~/qa/LastGit (feat2)
$ notepad readme.md

Admin@MIS MINGW64 ~/qa/LastGit (feat2)
$ git add readme.md

Admin@MIS MINGW64 ~/qa/LastGit (feat2)
$ git commit -m "Feature 2 branch added"
[feat2 604435a] Feature 2 branch added
 1 file changed, 5 insertions(+)

Admin@MIS MINGW64 ~/qa/LastGit (feat2)
$ git push
fatal: The current branch feat2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin feat2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Admin@MIS MINGW64 ~/qa/LastGit (feat2)
$ git push --set-upstream origin feat2
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Writing objects: 100% (3/3), 298 bytes | 298.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'feat2' on GitHub by visiting:
remote:      https://github.com/DeivisJ/lastGit/pull/new/feat2
remote:
To https://github.com/DeivisJ/lastGit.git
 * [new branch]      feat2 -> feat2
branch 'feat2' set up to track 'origin/feat2'.

Admin@MIS MINGW64 ~/qa/LastGit (feat2)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git branch feat3

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git checkout feat3
Switched to branch 'feat3'

Admin@MIS MINGW64 ~/qa/LastGit (feat3)
$ notepad readme.md

Admin@MIS MINGW64 ~/qa/LastGit (feat3)
$ git add readme.md

Admin@MIS MINGW64 ~/qa/LastGit (feat3)
$ git commit -m "feature 3 added"
[feat3 d5ed97f] feature 3 added
 1 file changed, 7 insertions(+)

Admin@MIS MINGW64 ~/qa/LastGit (feat3)
$ git push
fatal: The current branch feat3 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin feat3

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Admin@MIS MINGW64 ~/qa/LastGit (feat3)
$ git push --set-upstream origin feat3
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 295 bytes | 295.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'feat3' on GitHub by visiting:
remote:      https://github.com/DeivisJ/lastGit/pull/new/feat3
remote:
To https://github.com/DeivisJ/lastGit.git
 * [new branch]      feat3 -> feat3
branch 'feat3' set up to track 'origin/feat3'.

Admin@MIS MINGW64 ~/qa/LastGit (feat3)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git checkout git
error: pathspec 'git' did not match any file(s) known to git

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git checkout development
Switched to branch 'development'
Your branch is up to date with 'origin/development'.

Admin@MIS MINGW64 ~/qa/LastGit (development)
$ git merge feat3
Auto-merging readme.md
CONFLICT (content): Merge conflict in readme.md
Automatic merge failed; fix conflicts and then commit the result.

Admin@MIS MINGW64 ~/qa/LastGit (development|MERGING)
$ git push
Everything up-to-date

Admin@MIS MINGW64 ~/qa/LastGit (development|MERGING)
$ git add readme.md

Admin@MIS MINGW64 ~/qa/LastGit (development|MERGING)
$ git commit -m "Merging feature 3 to development"
[development 5c85242] Merging feature 3 to development

Admin@MIS MINGW64 ~/qa/LastGit (development)
$ git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 382 bytes | 382.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/DeivisJ/lastGit.git
   29de78c..5c85242  development -> development

Admin@MIS MINGW64 ~/qa/LastGit (development)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ notepad readme.md

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git add readme.md

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git commit -m "edited main readme"
[main 4c9032b] edited main readme
 1 file changed, 12 insertions(+)

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Writing objects: 100% (3/3), 282 bytes | 282.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/DeivisJ/lastGit.git
   6c9e972..4c9032b  main -> main

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git merge development
Auto-merging readme.md
CONFLICT (content): Merge conflict in readme.md
Automatic merge failed; fix conflicts and then commit the result.

Admin@MIS MINGW64 ~/qa/LastGit (main|MERGING)
$ git add readme.md

Admin@MIS MINGW64 ~/qa/LastGit (main|MERGING)
$ git commit -m "Merging development to main"
[main 18eb60e] Merging development to main

Admin@MIS MINGW64 ~/qa/LastGit (main)
$ git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 394 bytes | 394.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/DeivisJ/lastGit.git
   4c9032b..18eb60e  main -> main

