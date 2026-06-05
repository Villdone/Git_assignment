<img width="1230" height="584" alt="Screenshot 2026-06-05 165534" src="https://github.com/user-attachments/assets/dd3ab084-3675-4152-abc5-d9fe51854c90" /># Git & GitHub Assignment

For each **📸**, you must paste the terminal output or add a screenshot to this repository.

---

## Setup

Make sure you can read this file from GitHub.

Get two local clones of this GitHub repository (call them `Repo A` and `Repo B`). 
✋🏽 The rest of the assignment builds on top of this setup. Please make sure to get it right before moving on.

---

## Task 1: Local merge conflict

Set up a conflict entirely within Repo A: two branches with different changes on the same line, then merge them.

1. Setup: On your `main` branch, create a file named `conflict.txt`, add a line of text, and commit it.
2. Branch 1: Create and switch to branch `feature-left`. Modify that line of text, commit the change, and switch back to `main`.
3. Branch 2: From `main`, create and switch to branch `feature-right`. Modify that same line of text with a different change, and commit it.
4. The Merge: Switch back to `main`. Merge `feature-left` (this will succeed automatically), then try to merge `feature-right`.
5. The Fix: Git will flag a conflict. Open `conflict.txt`, look at the conflict markers, manually choose or combine the changes, and delete the markers. Save, stage (`git add`), and commit to finalize the merge.


### Deliverables
* 📸 The conflict markers in that particular file  
<img width="1422" height="164" alt="Screenshot 2026-06-05 163156" src="https://github.com/user-attachments/assets/fc0499a9-952a-4131-bdb6-4fc4ee0b83f4" />

* 📸 `git log --oneline` on `main` after resolving and merging
<img width="373" height="133" alt="Screenshot 2026-06-05 163319" src="https://github.com/user-attachments/assets/b1c03b6b-06eb-42b6-90be-6405a43fc7f0" />
---

## Task 2: Local and remote branches

Create a branch in Repo A, make a commit on it, and check from GitHub and Repo B whether it exists. Then push it and check again from Repo B. Switch to it in Repo B and make another commit.

### Deliverables
* 📸 `git branch -a` from Repo B **before** the push  82d1-ffa4955a7af6" />
<img width="560" height="311" alt="Screenshot 2026-06-05 164032" src="https://github.com/user-attachments/assets/f6e88c00-511a-4c21-8fa1-5f6a103ac2ac" />
<img width="523" height="185" alt="Screenshot 2026-06-05 163921" src="https://github.com/user-attachments/assets/d9f63a08-71e1-4cf2-b7e2-d113dfcfcf53" />
<img width="635" height="150" alt="Screenshot 2026-06-05 163650" src="https://github.com/user-attachments/assets/132a1690-db48-41de-8b03-e78b4139db3e" />

* 📸 `git branch -a` from Repo B **after** fetching  
* 📸 `git log --oneline` from Repo B checked out on that branch with one commit.


---
<img width="1488" height="1029" alt="Screenshot 2026-06-05 163500" src="https://github.com/user-attachments/assets/ed1e4a2e-4c2d-47f7-
## Task 3: Pull conflict

Create a merge conflict with Repo A and Repo B, with Repo A pushing first. Then try to push from Repo B. 

### Deliverables
* 📸 The push rejection message from Repo B  
* 📸 The conflict markers after pulling  <img width="622" height="373" alt="Screenshot 2026-06-05 164452" src="https://github.com/user-attachments/assets/200fb7d5-646b-4771-a023-f42017f62bfe" />
<img width="560" height="311" alt="Screenshot 2026-06-05 164032" src="https://github.com/user-attachments/assets/1807519b-1b2c-42ac-8804-09591869d4d8" />
<img width="1409" height="126" alt="Screenshot 2026-06-05 164129" src="https://github.com/user-attachments/assets/d737f3ad-9927-4178-98e8-6ed81ab80cfc" />

* 📸 `git log --oneline origin/main` (or a GitHub screenshot) after resolving

---

## Task 4: Don’t push secrets (.gitignore)

In **Repo A**, create a file that would normally contain secrets (for example `.env`) and put some obvious fake secret values in it (API key, password, etc.).

1. Confirm Git notices it (it should show as untracked).
2. Add that filename to `.gitignore`. (create this file first if necessary)
3. Confirm Git no longer lists it as untracked.
4. Commit and push **only** the `.gitignore` change (do **not** commit or push the secret file).

### Deliverables
* 📸 `git status` showing the secret file as untracked (before `.gitignore`)  
<img width="674" height="114" alt="Screenshot 2026-06-05 164655" src="https://github.com/user-attachments/assets/9a780fb2-8d92-423d-a1c0-8f2f12c18d0e" />
<img width="1064" height="244" alt="Screenshot 2026-06-05 164608" src="https://github.com/user-attachments/assets/1f3ff900-575c-45b0-9501-4aa0fb9c9a37" />
<img width="1221" height="459" alt="Screenshot 2026-06-05 164538" src="https://github.com/user-attachments/assets/08a60600-cfdb-496b-b751-dcd2b7d0e595" />

* 📸 `.gitignore` contents including your ignore rule  
* 📸 `git status` after adding `.gitignore` (showing the secret file is not listed)

---

## Task 5: Setup your project repo

Now work together with your group to setup your repository for the project.
- Make sure all team members have access to the repository
- Clone the repository to any location you like
- Set up the following branches
    - `main`
    - `dev`
    - `personal/[name]` for each team member 

### Deliverables
* 📸 `git branch -a` (or a GitHub screenshot) of your project repo completely setup.

<img width="322" height="99" alt="Screenshot 2026-06-05 165233" src="https://github.com/user-attachments/assets/21e7035b-400d-4aaa-964b-7ca8b82e6820" />
