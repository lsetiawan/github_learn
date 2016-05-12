# GitHub Tutorial Notes
## By Landung Setiawan
### Resource: http://rogerdudler.github.io/git-guide/

#### 1) Create a repository in GitHub and get link
- github_learn repository: https://github.com/lsetiawan/github_learn.git

#### 2) Make a new Directory and create new repository
- make new directory for files
```bash
$ mkdir github_learn
```
- Create
$ git init
```

#### 3) Connect local repository to remote server
```bash
$ git remote add origin https://github.com/lsetiawan/github_learn.git
```
- perform login by entering username and password

#### 4) Create a readme or other file and add to master branch in repo
1. **Create** the file
```bash
$ echo "# Learning Repository" >> README.md
```
2. **Add** file to staging (Index)
```bash
$ git add README.md
```
3. **Commit** changes
```bash
$ git commit -m "Commit Message"
```
4. **Push** file to master branch
```bash
$ git push origin master
```

#### 5) Branching
- **List** all Branches (Local and Remote)
```bash
$ git branch -a
```
- **Create** a Branch
```bash
$ git checkout -b branch_name
```
- **Delete** a Branch
```bash
$ git branch -d branch_name
```
- **Sync** branch list (local and remote)
```bash
$ git fetch -p
```
- **Push** Branch to remote repo
```bash
$ git push origin branch_name
```
- **Switch** Branches
``` bash
$ git checkout branch_name
```

#### 6) Update and Merge
- Update local repository to the newest Commit (fetch and merge remote changes)
```bash
$ git pull
```
- Compare Branches before merging
```bash
$ git diff source_branch target_branch
```
- Merge another branch into active branch
```bash
$ git merge branch_name
```

#### 7) Replace local changes
- replaced with the last content in HEAD (commit before push)
```bash
$ git checkout -- README.md
```
