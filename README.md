# Git & GitHub Exercises

## **Task 1: Version Control & Branching**

### **Objective:**
Learn the basics of version control by creating a repository, working with branches, and making pull requests.

### **Steps:**
1. Create a new Git repository on GitHub (or any Git hosting service).
2. Clone the repository locally.
3. Navigate to the repository directory.
4. Create a new branch called `feature-update`.
5. Add a new file named `README.md` and write a short introduction about yourself.
6. Stage and commit the changes.
7. Push the `feature-update` branch to the remote repository.
8. Open a pull request (PR) on GitHub to merge `feature-update` into `main`.
9. Merge the PR after reviewing changes.

### **Solution:**
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
![GitHub Logo](https://files.fm/f/xqbhtzks37)


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
![pull request](https://files.fm/f/rb7pf6uhth)

---

## **Task 2: Team Collaboration (Pair Programming)**

### **Objective:**
Collaborate with another student using GitHub’s collaboration features.

### **Steps:**
1. One student creates a new repository and invites a team member as a collaborator.
2. The repository owner creates an `index.html` file and pushes it to `main`.
3. The collaborator clones the repository.
4. The collaborator creates a new branch `update-styles`.
5. Modify `index.html` by adding a `<style>` section.
6. Commit and push the changes.
7. Open a pull request.
8. The repository owner reviews, approves, and merges the PR.
9. Both students pull the latest changes.

### **Solution:**
... *(Similar step-by-step breakdown with placeholders for images and expected outcomes)* ...

### **Expected Outcome:**
![Collaboration Example](image_placeholder)

---

## **Task 3: Resolving Merge Conflicts**

### **Objective:**
Learn how to resolve merge conflicts when merging branches.

### **Steps:**
1. Each student creates a repository and clones it.
2. Create a new branch `edit-text`.
3. Modify an existing file (or create one) and commit the changes.
4. Switch back to `main`.
5. Modify the same file in a different way and commit.
6. Merge `edit-text` into `main`.
7. Resolve any merge conflicts manually and commit the changes.
8. Push the final changes to the repository.

### **Expected Outcome:**
![Merge Conflict Resolution Example](image_placeholder)

---

## **Task 4: Working with a Remote Repository**

### **Objective:**
Contribute to an open-source project by forking, making changes, and submitting a pull request.

### **Steps:**
1. Fork a repository from a popular open-source project on GitHub.
2. Clone the forked repository.
3. Navigate to the repository directory.
4. Create a new branch called `documentation-update`.
5. Make meaningful changes to the documentation files.
6. Stage and commit the changes.
7. Push the branch to your fork.
8. Create a pull request to the original repository.
9. Document the process and any feedback received.

### **Expected Outcome:**
![Open Source Contribution Example](image_placeholder)

---


