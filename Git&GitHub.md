## Local Git
Local git repos have 3 componets:
* Working directory - The directory the file is in
* Index - used in staging
* Head - points to the commit

These componets work in this structure:
![](https://blog.udemy.com/wp-content/uploads/2015/08/image036.png)

### Cloning a file down from GitHub

To get your most recent master/branch, use the code `git clone <http://repourl.git>` This will give you a full, complete and up-to-date version of the latest file push.

### Adding

All files are either *tracked*, that is, staged such that you could commit any changes they have, or *untracked*, where any changes you have made are not prepared to be committed. 

You can "track" files by using the code `git add <filename>` 

git does not continuously track files that have been added. At the time of commit, it takes a snapshot of your changes in comparison to the latest commit. You can create a snapsot of your changes by committing your code.

### Committing 

A committed file has had a snapshot of it's most recent changes made for version control purposes. All commits should have a brief message stating briefly what changes were made. Committing your changes is as simple as `git commit <filename>`

**Note: You should be continuously adding/committing your work as you go. Save your work, nerd!**

### Making sure you're good to go

`git status` is your friend. You should be checking your status with every add, commit and push.

### Pushing

Pushing your changes back up to your GitHub repo is as simple as `git push`. Enter your credentials, if necessary, and push your changes.

