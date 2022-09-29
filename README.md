# GitHub - Create Local Repository and Push to GitHub

## 1) Add Local Repo

Create local repo named <strong>local_repo</strong>, then create a new file named <strong>test.txt</strong> and add some content in it (requirement because will not be able to push an empty folder).

```bash
mkdir local_repo
cd local_repo
vi test.txt
```

## 2) Run <em>git init</em> command

This will convert our working directory into a GitHub Repo.
It will create a <strong>.git</strong> folder.

```bash
git init
```

## 3) Stage all changes made and then commit

```bash
git add .
git commit -m "1st commit"
```

## 4) Now open GitHub portal and create new repo

Go to <em>https://github.com/</em> and create new repo.
Name your repo <strong>Test</strong> under Repository name. Can skip all optional settings and click on <strong>Create Repository</strong> button.
This will create an empty repo.

## 5) Add remote URL

Copy link of repo (https adress) and paste it after the <strong><em>git remote add origin</em></strong> command:

```bash
git remote add origin https://github.com/jkoubs/Test.git
```

The git on your local machine needs to know which repo on GitHub (remote) is linked to it. With this command, we had a remote URL.

The word <strong>origin</strong> is a nickname of the remote repo (can choose any name you like).

## 6) Push to Github

Now, we can <strong>push</strong> the changes to the <strong>master</strong> branch of the <strong>origin</strong>.

```bash
git push origin master
```

<strong><u><em>Note</em></u></strong>:  Can use a short form of the <strong><em>git push</em></strong> command by running:

```bash
git push --set-upstream origin master
git push
```
With this we can now run <strong><em>git push</em></strong> instead of <strong><em>git push origin master</em></strong>.
It is a shortcut that will push to the <strong>master</strong> branch

## 7) Refresh GitHub page 

Go back to GitHub webpage and refresh the page to confirm the repo has been pushed correctly.