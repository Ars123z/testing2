status of files
============================

1. Untracked
2. Unmodified
3. Modified
4. Staged


git status
======================

1. On branch main -> always
2. No commits yet -> if nothing is commited so far
3. nothing to commit (untracked file present)-> if no file is currently staged for commit and (there are untracked files)
4. Untracked files: -> if there are untracked files present
5. Changes to be commited -> if there is any staged file
6. Changes not staged for commit -> if a tracked file is modified but not added (a file a can appear in both 5 and 6 if a added but not commited file is changed)

Rules for .gitignore file
==========================

1. Blank lines or lines atarting with # are ignored
2. Standard glob patterns work, and will be applied recursively throughout the entire working tree.
3. You can start patterns with a forward slash (/) to avoid recursivity.
4. You can end patterns with a forward slash (/) to specify a directory.
5. You can negate a pattern by starting it with an exclamation point (!).

glob pattern
===========================

1. * -> Matches zero or more characters
2. [abc] -> Matches any character in the bracket.
3. ? -> Matches single character
4. [0-9] -> Matches any character between them
5. a/**/z -> Matches nested directory

git diff
========================

1. git diff -> show difference between working directory and staging area return nothing if no changes

2. git diff --staged -> show difference between staging area and the previous commit

git restore <file>
====================
restore the changed file to the staged version
unstage file with --staged flag

git rm <file>
========================
remove the file from git as well as from the editor. Get the file to untracked with --cached flag

git mv <file> <file>
=========================
rename the file

git log [--patch --stat --preety=oneline]
===========================
1. showes commit history and diff output if used with patch option
2. abbreviated changes in each commit
3. All logs in one line when used with preety=oneline option

git commit [--amend]
============================
1. commit staged file
2. replace the last commit with new commit

git reset Head <file>
========================

1. to unstage a staged file


git remote 
=============================
1. git remote -> list all the remote
2. git remove -v -> list all the remotes with fetch/pull url
3. git remote add <nickname> url -> add new remote
4. git remote show <nickname> -> for more info
5. git fetch <nickname> -> fetches all changes not reflect in theworking directory untill merged
6. git pull -> fetches all changes and tries to merge if tracking is set
7. git push <nickname> <branch>
8. git remote remove -> remove the remote 
9. git remote rename <nickname> <newname>

<!-- this is a comment -->

