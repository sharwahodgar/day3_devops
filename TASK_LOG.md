# TASK 4: DevOps Project Version Control Log

This document records the steps taken to build and manage the project repository using Git best practices, as required by the task.

## Phase 1: Initialization and Setup (Hints a, d)

| Step | Action Performed | Git Commands Used | Outcome |
| :--- | :--- | :--- | :--- |
| **1** | Initialized the local Git repository. | `git init` | Git tracking started. |
| **2** | Created the **README.md** file. | (File creation) | Documentation added (Hint d). |
| **3** | Linked the local repository to GitHub. | `git remote add origin <link>` | Project connected to online repo (Hint a). |
| **4** | Created and pushed the first commit. | `git add .` <br> `git commit -m "Initial commit: Added README"` <br> `git branch -M main` <br> `git push -u origin main` | **main** branch established on GitHub (Hint a). |

***

## Phase 2: Branching and Feature Development (Hints b, e)

| Step | Action Performed | Git Commands Used | Outcome |
| :--- | :--- | :--- | :--- |
| **5** | Created and switched to the **dev** branch. | `git branch dev` <br> `git checkout dev` | Set up the main development line (Hint b). |
| **6** | Created a specific feature branch. | `git checkout -b feature/add-ignore` | Started work on a new isolated task (Hint b). |
| **7** | Added the **.gitignore** file. | (File creation with `*.log`) | Configured Git to ignore unnecessary files (Hint e). |
| **8** | Committed and pushed the new feature. | `git add .gitignore` <br> `git commit -m "FEAT: Added .gitignore file"` <br> `git push -u origin feature/add-ignore` | Feature changes saved and sent to GitHub. |

***

## Phase 3: Review and Final Release (Hints c, e)

| Step | Action Performed | Git Commands Used | Outcome |
| :--- | :--- | :--- | :--- |
| **9** | **Merged** feature into **dev**. | (Used **Pull Request** on GitHub) | Feature code was reviewed and integrated (Hint c). |
| **10** | Synced the local **dev** branch. | `git checkout dev` <br> `git pull origin dev` | Local development line updated. |
| **11** | **Merged** **dev** into **main**. | (Used **Pull Request** on GitHub) | Final, stable code moved to the main branch (Hint c). |
| **12** | Tagged the stable code as a release. | `git checkout main` <br> `git tag v1.0` <br> `git push origin v1.0` | Marked the version as v1.0 (Hint e). |
| **13** | Documented all steps in this file. | (File creation) | Completed documentation task (Hint f). |