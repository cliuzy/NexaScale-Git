# NexaScale-Git
___

# Git & GitHub Exercises

## **Task 1: Version Control & Branching**

1. Create a new Git repository on GitHub (or any Git hosting service).
   - **Expected Result:** A new repository is created on GitHub.
2. Clone the repository locally:
   ```sh
   git clone <repository_url>
   ```
   - **Expected Result:** The repository is copied to your local machine.
3. Navigate to the repository directory:
   ```sh
   cd <repository_name>
   ```
   - **Expected Result:** You are inside the repository folder.
4. Create a new branch called `feature-update`:
   ```sh
   git checkout -b feature-update
   ```
   - **Expected Result:** A new branch named `feature-update` is created and checked out.
5. Add a new file named `README.md` and write a short introduction about yourself.
6. Stage and commit the changes:
   ```sh
   git add README.md
   git commit -m "Added README with introduction"
   ```
   - **Expected Result:** Changes are staged and committed to the `feature-update` branch.
7. Push the `feature-update` branch to the remote repository:
   ```sh
   git push origin feature-update
   ```
   - **Expected Result:** The `feature-update` branch is uploaded to GitHub.
8. Open a pull request (PR) on GitHub to merge `feature-update` into `main`.
   - **Expected Result:** A PR is created and visible on GitHub.
9. Merge the PR after reviewing changes.
   - **Expected Result:** The `feature-update` branch is merged into `main`.

---

## **Task 2: Team Collaboration (Pair Programming)**

1. One student should create a new repository and invite a team member as a collaborator.
   - **Expected Result:** The repository exists with the collaborator added.
2. The repository owner creates an `index.html` file and pushes it to `main`:
   ```sh
   echo "<html><body><h1>Welcome</h1></body></html>" > index.html
   git add index.html
   git commit -m "Initial commit with index.html"
   git push origin main
   ```
   - **Expected Result:** `index.html` is available in the remote repository.
3. The collaborator clones the repository:
   ```sh
   git clone <repository_url>
   ```
   - **Expected Result:** The repository is copied to their local machine.
4. The collaborator creates a new branch `update-styles`:
   ```sh
   git checkout -b update-styles
   ```
   - **Expected Result:** A new branch named `update-styles` is created.
5. Modify `index.html` by adding a `<style>` section.
6. Commit and push the changes:
   ```sh
   git add index.html
   git commit -m "Added styles to index.html"
   git push origin update-styles
   ```
   - **Expected Result:** Changes are uploaded to GitHub in `update-styles`.
7. Open a pull request.
   - **Expected Result:** A PR is created on GitHub.
8. The repository owner reviews, approves, and merges the PR.
   - **Expected Result:** The changes are merged into `main`.
9. Both students pull the latest changes:
   ```sh
   git checkout main
   git pull origin main
   ```
   - **Expected Result:** Both contributors have the latest version locally.

---

## **Task 3: Resolving Merge Conflicts**

1. Each student creates a repository and clones it.
2. Create a new branch `edit-text`:
   ```sh
   git checkout -b edit-text
   ```
   - **Expected Result:** A new branch `edit-text` is created.
3. Modify an existing file (or create one) and commit the changes.
4. Switch back to `main`:
   ```sh
   git checkout main
   ```
5. Modify the same file in a different way and commit.
6. Merge `edit-text` into `main`:
   ```sh
   git merge edit-text
   ```
   - **Expected Result:** A merge conflict occurs (if changes conflict).
7. If a merge conflict occurs, manually resolve it, then commit the final version:
   ```sh
   git add <file_name>
   git commit -m "Resolved merge conflict"
   ```
   - **Expected Result:** Conflict is resolved and committed.
8. Push the final changes to the repository:
   ```sh
   git push origin main
   ```
   - **Expected Result:** The updated `main` branch is pushed to GitHub.

---

## **Task 4: Working with a Remote Repository**

1. Fork a repository from a popular open-source project on GitHub.
   - **Expected Result:** The repository appears under your GitHub account.
2. Clone the forked repository:
   ```sh
   git clone <forked_repository_url>
   ```
   - **Expected Result:** The forked repository is copied to your local machine.
3. Navigate to the repository directory:
   ```sh
   cd <repository_name>
   ```
4. Create a new branch called `documentation-update`:
   ```sh
   git checkout -b documentation-update
   ```
   - **Expected Result:** A new branch `documentation-update` is created.
5. Make meaningful changes to the documentation files (`README.md`, `CONTRIBUTING.md`, etc.).
6. Stage and commit the changes:
   ```sh
   git add .
   git commit -m "Updated documentation"
   ```
   - **Expected Result:** Changes are saved in the local branch.
7. Push the branch to your fork:
   ```sh
   git push origin documentation-update
   ```
   - **Expected Result:** The `documentation-update` branch is available on GitHub.
8. Create a pull request to the original repository.
   - **Expected Result:** A PR is opened for review.


---



