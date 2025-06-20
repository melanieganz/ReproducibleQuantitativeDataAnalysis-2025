# Step 1

```bash
git config --global user.name "GitHubUserName"   
git config --global user.email "YourEmail"
```

# Step 2

```bash
cd /path/to/your/desired/location
mkdir my-new-repo
cd my-new-repo
git init
ls -la
cd .git
ls -la
cd ..
```

# Step 3

cut/paste MyFirstMarkdownFile.md into your new folder

```bash
git status
git add .
git commit -m "my first commit"
```
Change something in your markdown
```bash
git log --oneline
git restore MyFirstMarkdownFile.md
```

# Step 4

Create a file 
```bash
touch tmpinfo.txt
```

Create a folder and file notes/notes.md
```bash
mkdir notes
cd notes
touch notes.md
cd ..
```

Now create a .gitignore file, and let's edit it as to ignore what we want to ignore (use wild card for folder contend)
```bash
touch .gitignore
echo "tmpinfo.txt" >> .gitignore
echo "notes/*" >> .gitignore
```

for Mac you can ignore .DS_Store but cached stuff is annoying, do  
```
git rm --cached .DS_Store
```

# Step 5

Fork the course repository to your own GitHub account, then using GitHub Desktop, clone your forked repository to your local machine.
Overwrite the MyFirstMarkdownFile.md file from the course repository with your own version.

```bash
cd folder/where/you/cloned/your/repo
git status
git add .
git commit -m "Overwrite MyFirstMarkdownFile.md with my own version"
git push 
```

# Step 6

Now you'll do a pull request to the course repository.
Go to the repository on GitHub, and click on the "Pull requests" tab. Click on "New pull request". Select the course and the forked repositories. Add a title and description, then click "Create pull request".
