# Steps to use git

1. install git from this [link](https://gitforwindows.org/)

2. then configer git in you pc or laptop.

2. make a folder in your hard drive locally

3. got to that folder via command prompt or terminal
```git
cd <pathtofolder>
```

4. initialize git repository
```
git init
```

5. add changes to the stage changes in single file.

```
git add <path_to_file>
```
or, use this command to stage all changes at once in multiple files.
```
git add .
```

6. commit the changes if you are done with changes: 
(note: always write massage because it will help in tracking your commits history in future.)
```
git commit -m "yourmessage"
```

7. to sync changes use this:
```
git push <remote name> <branch name>
```
note:(defualt remote name is "origin" and also use as best practice too. and defualt branch name is "master" in git and "main" in github.
both remote and branch names can be change as per need.) 