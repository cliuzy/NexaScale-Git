# Git & GitHub Exercises

## **Task 1: Version Control & Branching**

### **Objective:**
Learn the basics of version control by creating a repository, working with branches, and making pull requests.


#### Step 1: Create a repository
- Navigate to GitHub and create a new repository "NexaScale-Git"

#### Step 2: Clone the repository
```sh
git clone https://github.com/cliuzy/NexaScale-Git
```
**Expected Result:** The repository is copied to your local machine.

#### Step 3: Navigate to the repository directory
```sh
cd Nexascale
```

#### Step 4: Create a new branch
```sh
git checkout -b feature-update
```
**Expected Result:** A new branch named `feature-update` is created and checked out.
![](https://raw.githubusercontent.com/cliuzy/NexaScale-Git/main/images/sc2.png)





#### Step 5: Add a new file and write an introduction
```sh
echo "# My Introduction" > README.md
```

#### Step 6: Stage and commit the changes
```sh
git add README.md
git commit -m "Added README with introduction"
```


#### Step 7: Push the branch to remote
```sh
git push origin feature-update
```
**Expected Result:** The branch is uploaded to GitHub.

#### Step 8: Open a PR on GitHub
- Navigate to GitHub and open a pull request.

#### Step 9: Merge the PR
- Review changes and merge the branch into `main`.

### **Expected Outcome:**
![pull request](https://raw.githubusercontent.com/cliuzy/NexaScale-Git/main/images/sc1.png)


---

## **Task 2: Team Collaboration (Pair Programming)**

### **Objective:**
Collaborate with another student using GitHub’s collaboration features.

#### Step 1: Repository owner creates a new repository and invites a collaborator
- Navigate to GitHub and create a new repository.
- Go to **Settings > Collaborators** and invite the team member.

#### Step 2: Repository owner creates and pushes `index.html`
```sh
echo "<html><body><h1>Welcome</h1></body></html>" > index.html
git add index.html
git commit -m "Initial commit with index.html"
git push origin main
```
**Expected Result:** `index.html` is available in the remote repository.

#### Step 3: Collaborator clones the repository
```sh
git clone <repository_url>
```
**Expected Result:** The repository is copied to the collaborator's local machine.

#### Step 4: Collaborator creates a new branch `update-styles`
```sh
git checkout -b update-styles
```
**Expected Result:** A new branch `update-styles` is created.

#### Step 5: Modify `index.html` by adding a `<style>` section
```sh
echo "<style> body { background-color: lightblue; } </style>" >> index.html
```

#### Step 6: Commit and push the changes
```sh
git add index.html
git commit -m "Added styles to index.html"
git push origin update-styles
```
**Expected Result:** Changes are uploaded to GitHub in `update-styles`.

#### Step 7: Open a PR
- Navigate to GitHub and create a pull request from `update-styles` to `main`.

#### Step 8: Repository owner reviews, approves, and merges the PR
- Review the changes and merge the PR.

#### Step 9: Both students pull the latest changes
```sh
git checkout main
git pull origin main
```
**Expected Result:** Both contributors have the latest version locally.
### **Expected Outcome:**
![pull request](https://raw.githubusercontent.com/cliuzy/NexaScale-Git/main/images/sc5.png)

---
# Task 3 - resolving conflict
## **Step 1: Create and Clone a Repository

```markdown
# **Resolving Merge Conflicts in Git**

## **Step 1: Create and Clone a Repository**  
```bash
git init merge-conflict-demo
cd merge-conflict-demo
echo "This is the original content." > conflict.txt
git add conflict.txt
git commit -m "Initial commit"
```

---

## **Step 2: Create and Modify a New Branch**  
```bash
git checkout -b edit-text
echo "This is the edit-text branch modification." > conflict.txt
git commit -am "Updated conflict.txt in edit-text branch"
```

---

## **Step 3: Modify `main` Branch **  
```bash
git checkout main
echo "This is the main branch modification." > conflict.txt
git commit -am "Updated conflict.txt in main branch"
```

---

## **Step 4: Merge and Create a Conflict**  
```bash
git merge edit-text
```
Git will detect conflicting changes and show a message like:  
```plaintext
Auto-merging conflict.txt
CONFLICT (content): Merge conflict in conflict.txt
```
![](https://raw.githubusercontent.com/cliuzy/NexaScale-Git/main/images/sc2.png)

---

## **Step 5: Resolve the Merge Conflict**  
1. Open `conflict.txt`, and you'll see markers like:
    ```plaintext
    <<<<<<< HEAD
    This is the main branch modification.
    =======
    This is the edit-text branch modification.
    >>>>>>> edit-text
    ```
2. Choose the correct content or manually merge them:  
    ```plaintext
    This is the merged version, combining both changes.
    ```
3. Save the file.

---

## **Step 6: Commit and Push the Resolved Version**  
```bash
git add conflict.txt
git commit -m "Resolved merge conflict"
git push origin main
```
![](https://raw.githubusercontent.com/cliuzy/NexaScale-Git/main/images/sc3.png)





---




