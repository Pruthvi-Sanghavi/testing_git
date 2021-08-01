# This repository is used to test various git functions and document them

## Make a new repository from terminal
```
git init -b <branch_name>
git add .
git commit -m "Comment Here"
```

If you haven't configured github with Ubuntu. It will give the message,
```
Author identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

```
Add commit if you havent already done that because of the error
```
git commit -m "Your comment"
git remote add origin https://github.com/Pruthvi-Sanghavi/testing_git.git
git remote -v
git push origin devel 
```
Now if you are using the old commit method then your git credentials wont work. 
```
pruthvi@pruthvi:~/testing_git (git: devel)$ git push origin devel 
Username for 'https://github.com': Pruthvi-Sanghavi
Password for 'https://Pruthvi-Sanghavi@github.com': 
remote: Invalid username or password.
```
In this case, head to your github homepage
```
Setting > Developer Settings > Personal Access Token > Generate new token
```
You have to select some rights and permissions and a new token will get generated.\
### Copy that token as you see it and save it somewhere as you will not see that again.
Add your account details and boom!
```
pruthvi@pruthvi:~/testing_git (git: devel)$ git push origin devel 
Username for 'https://github.com': Pruthvi-Sanghavi
Password for 'https://Pruthvi-Sanghavi@github.com': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 3.41 KiB | 1.13 MiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Pruthvi-Sanghavi/testing_git.git
 * [new branch]      devel -> devel

```

## Creating a new branch and commiting the files

Check that you are on the new branch
```
git checkout devel
```
Create a new branch,
```
git checkout -b user/pruthvi-sanghavi/test-branch
```
Check the new branch using
```
git branch
```
Commit and push the branch.

## Checking a few things like merging without updating the devel(default) branch

- This process works ok. You just need to go to the repository and merge the changes.

## Merging changes by a contributor

- Added a new file
```
The process is pretty straight forward
```

- Adding a change to existing file.
```
The process looks the same but lets see
```











