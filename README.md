# versionControl

[mashraf@localhost version_control]$ git commit -m "lab2 added"
[master f7707e0] lab2 added
 Committer: mohamed ashraf <mashraf@localhost.localdomain>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 lab2.html
[mashraf@localhost version_control]$ git push origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 278 bytes | 10.00 KiB/s, done.
Total 2 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:mohamedashraf206/versionControl.git
   4003e3a..f7707e0  master -> master
[mashraf@localhost version_control]$ git commit -m "lab2 edited"
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   lab2.html

no changes added to commit (use "git add" and/or "git commit -a")
[mashraf@localhost version_control]$ git commit -am "lab2 edited"
[master cec87fd] lab2 edited
 Committer: mohamed ashraf <mashraf@localhost.localdomain>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 12 insertions(+)
[mashraf@localhost version_control]$ git push origin master
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 430 bytes | 430.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:mohamedashraf206/versionControl.git
   f7707e0..cec87fd  master -> master
[mashraf@localhost version_control]$ git branch myBranch1
[mashraf@localhost version_control]$ git status
On branch master
nothing to commit, working tree clean
[mashraf@localhost version_control]$ git checkout myBranch1
Switched to branch 'myBranch1'
[mashraf@localhost version_control]$ git branch -d myBranch1
error: Cannot delete branch 'myBranch1' checked out at '/home/mashraf/version_control'
[mashraf@localhost version_control]$ git branch dev
[mashraf@localhost version_control]$ git checkout dev
Switched to branch 'dev'
[mashraf@localhost version_control]$ git branch -d myBranch1
Deleted branch myBranch1 (was cec87fd).
[mashraf@localhost version_control]$ git branch
* dev
  master
[mashraf@localhost version_control]$ git branch test
[mashraf@localhost version_control]$ git branch
* dev
  master
  test
[mashraf@localhost version_control]$ git checkout master
Switched to branch 'master'
[mashraf@localhost version_control]$ git diff
[mashraf@localhost version_control]$ git branch -r
  origin/master
[mashraf@localhost version_control]$ git branch
  dev
* master
  test
[mashraf@localhost version_control]$ git checkout dev
Switched to branch 'dev'
[mashraf@localhost version_control]$ git status
On branch dev
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   lab2.html

no changes added to commit (use "git add" and/or "git commit -a")
[mashraf@localhost version_control]$ git commit -am "file is edited on dev branch"
[dev b91b9af] file is edited on dev branch
 Committer: mohamed ashraf <mashraf@localhost.localdomain>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+), 1 deletion(-)
[mashraf@localhost version_control]$ git checkout master
Switched to branch 'master'
[mashraf@localhost version_control]$ git branch
  dev
* master
  test
[mashraf@localhost version_control]$ git checkout dev
Switched to branch 'dev'
[mashraf@localhost version_control]$ git checkout master
Switched to branch 'master'
[mashraf@localhost version_control]$ git checkout dev
Switched to branch 'dev'
[mashraf@localhost version_control]$ git push origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 341 bytes | 341.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/mohamedashraf206/versionControl/pull/new/dev
remote: 
To github.com:mohamedashraf206/versionControl.git
 * [new branch]      dev -> dev
[mashraf@localhost version_control]$ git add
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Turn this message off by running
hint: "git config advice.addEmptyPathspec false"
[mashraf@localhost version_control]$ git add .
[mashraf@localhost version_control]$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        deleted:    file.text
        deleted:    index.html

[mashraf@localhost version_control]$ git commit -m "delete 2 file"
[dev fe160dd] delete 2 file
 Committer: mohamed ashraf <mashraf@localhost.localdomain>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 2 files changed, 22 deletions(-)
 delete mode 100644 file.text
 delete mode 100644 index.html
[mashraf@localhost version_control]$ git push origin dev
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 12 threads
Compressing objects: 100% (1/1), done.
Writing objects: 100% (2/2), 237 bytes | 237.00 KiB/s, done.
Total 2 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:mohamedashraf206/versionControl.git
   b91b9af..fe160dd  dev -> dev
[mashraf@localhost version_control]$ git checkout test
Switched to branch 'test'
[mashraf@localhost version_control]$ git add .
[mashraf@localhost version_control]$ git commit -m "new paragraph delete 2 [test ec6a6ad] new paragraph delete 2 file
 Committer: mohamed ashraf <mashraf@localhost.localdomain>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 3 files changed, 4 insertions(+), 23 deletions(-)
 delete mode 100644 file.text
 delete mode 100644 index.html
[mashraf@localhost version_control]$ git push origin test
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 373 bytes | 373.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/mohamedashraf206/versionControl/pull/new/test
remote: 
To github.com:mohamedashraf206/versionControl.git
 * [new branch]      test -> test
[mashraf@localhost version_control]$ git checkout master
Switched to branch 'master'
[mashraf@localhost version_control]$ git merge dev -m "dev is merged to the
master"
Updating cec87fd..fe160dd
Fast-forward (no commit created; -m option ignored)
 file.text  | 22 ----------------------
 index.html |  0
 lab2.html  |  2 +-
 3 files changed, 1 insertion(+), 23 deletions(-)
 delete mode 100644 file.text
 delete mode 100644 index.html
[mashraf@localhost version_control]$ git push origin master
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:mohamedashraf206/versionControl.git
   cec87fd..fe160dd  master -> master
[mashraf@localhost version_control]$ git merge test -m  "test is merged to the master branch"
Auto-merging lab2.html
CONFLICT (content): Merge conflict in lab2.html
Automatic merge failed; fix conflicts and then commit the result.
[mashraf@localhost version_control]$ git merge dev -m "dev is merged to the mhehmaster"
error: Merging is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
[mashraf@localhost version_control]$ git merge test -m  "test is merged to the mhmaster branch"
error: Merging is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
[mashraf@localhost version_control]$ git merge test -m  "test is merged to the mtmaster branch"
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.
[mashraf@localhost version_control]$ git commit -am "merging"
[master d3e6f0d] merging
 Committer: mohamed ashraf <mashraf@localhost.localdomain>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

[mashraf@localhost version_control]$ git status
On branch master
nothing to commit, working tree clean
[mashraf@localhost version_control]$ git push origin master
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 315 bytes | 315.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:mohamedashraf206/versionControl.git
   fe160dd..d3e6f0d  master -> maste
