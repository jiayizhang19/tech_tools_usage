### Initial Git Setup on a New Machine:

1. Setup git user and email
    ```
    git config --global user.name "name"
    git config --global user.email "github email"
    ```
    command to change login user:
    ```
    git commit --amend --reset-author
    ```

2. Check current user
    ```
    git config --global --list
    ```

3. Generate ssh key
    ```
    ssh-keygen -t ed25519 -C "gitHub email"
    ```

4. Add public key to Github

5. Check ssh configuration with returned message "Hi your-username! You've successfully authenticated..."
    ```
    ssh -T git@github.com
    ```

### Git Phases
1. Initialization: start a git repository  
    --> git init   
    --> git clone
2. Working area (Untracked Changes)  
    --> git status  
    --> This is where you create, modify or delete files. Git knows about the files but hasn't started tracking the changes yet.  
3. Staging Area (Staged Changes)  
    --> git add [file_name] or git add .  
    --> This is where you define which changes should be saved in the next commit by staging them  
4. Local Repository (Tracked Changes)  
    --> git commit -m "message"  
    --> This is where your staged changes are saved as a commit, which acts as a snapshot of your project at that moment.  
5. Remote Repository (Tracked Changes)
    --> git push  
    --> This is where you push your commits to a remote repo to share or back up your work.  

### Git Branches
1. Show all local branches
    ```
    git branch 
    ```
2. Show all remote branches
    ```
    git branch -r
    ```
3. Create a new branch xxx
    ```
    git branch xxx
    ```
4. Switch to an existing branch xxx
    ```
    git checkout xxx
    ```
5. Rename the current branch to xxx
    ```
    git branch -m xxx  
    ```
6.Delete a local branch xxx  
    ```
    git branch -d xxx  
    ```

### 



