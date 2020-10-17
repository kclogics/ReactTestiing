centeralized git
distributed(git)

1. git config --global user.name "kclogics"
2. git config --global user.email "kclogics@gmail.com"
3. git config --global core.editor "code --wait"

<!-- gitconfig file ------------------------------------------------->

git config --global -e

<!-- if you are on linux/mac (folderpath) -->

git config --global core.autocrlf input

<!-- if you are on windows (folder path) -->

git config --global core.autocrlf true

<!-- help ------------------------------------------------------------>

git config -h

<!--  -->

1. git init
2. git status
3. git add file1.txt file2.txt
4. echo >> file1.txt hello js
5. echo test >> file1.txt
6. git commit -am "skipp the stagging"
7. git ls-files <!--staging area ->
8. git rm file2.txt \*.txt

9. git checkout path/to/filename <!-- retreat deleted file -->
10. git checkout HEAD^ path/to/filename <!-- retreat deleted file -->
11. git checkout HEAD^ path/to/filename <!-- retreat deleted file -->
12. mv main.js index.md <!--change file name -->
13. git mv index.md main.md <!--change file name applied to sttaging -->

<!--  ---------------------------------------------------------------->
<!-- git ignore-->

1. mkdir logs
2. echo hello > log\dev.log
3. echo logs\ > .gitignore
4. mkdir bin
5. echo hello > bin\app.bin
6. git status
<!-- git ls-files <!--staging area -> -->
7. git rm -h
8. git rm --cached -r bin/ <!--Remove files from staging area if u added then with git add-->

<!--  -->

9. https://github.com/github/gitignore <!-- all the git ignore files->
<!--  -->
10. echo sky >> file1.js
11. echo sky >> file2.js

<!-- diff -->

12. git diff
13. git diff --staged

<!--visual git  -->

14. git config --global diff.tool vscode
15. git config --global difftool.vscode.cmd "code --wait --diff $LOCAL $REMOTE"
16. git config --global -e
17. git difftool
18. git difftool --staged
    <!--  -->
    git log --oneline
    git log --oneline --reverse
19. git show c822276
20. git show HEAD~1
21. git show HEAD~1: .gitignore
22. git ls-tree HEAD~1
    <!--  -->
    Commits
    Blobs(Files)
    Trees(Directories)
    <!--  -->
    <!--  -->
23. git update
24. git reset <!--confusion -->
25. git reset --hard
26. git reset --soft

27. git restore --staged file1.js <!--  git reset alternative , work only in latest git -->
<!-- git status -s -->
28. git restore .
29. git clean -fd
30. git restore --source=HEAD~1 file.js
31. git restore --source=HEAD file.js
32. git log --oneline
33. git commit --amend <!--commit in the dsame commit -->
34. git merge branchname
35. git merge --abort
