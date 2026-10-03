git add is when i put the changes in the staging area, like getting them ready

git commit is when i seal those staged changes into a commit

-m "..." lets me give the commit a message so i know what the commit was about, the quotes keep the whole message together as one argument

branch is more like a separate timeline not a full copy of the whole project, this matters because i can make changes on one branch without changing the other branch

git branch <name> creates the new branch but doesn't move me to it

git switch <name> moves me to that branch, the * showed which branch i was currently on

in the lab i added a line to the README on experiment and when i went back to main that line wasn't there, showing that the branches had their own changes

the a01cc35 mix-up was about not being sure what that commit actually contained, instead of guessing i used git show to check the commit and see what changes it had

one mistake was confusing creating a branch with switching to it, because git branch creates it but keeps you on the current branch
