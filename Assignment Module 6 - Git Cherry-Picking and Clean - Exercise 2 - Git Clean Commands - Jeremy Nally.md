# Assignment Module 6 - Git Cherry-Picking and Clean - Exercise 2 - Git Clean Commands - Jeremy Nally

* **Preview the changes:** `git clean -n` (or `--dry-run`)
    * **Description:** Performs a "dry run" to preview which untracked files will be deleted without actually removing them.
* **Remove Untracked Files:** `git clean -f` (or `--force`)
    * **Description:** Forcibly removes untracked files from the current working directory.
* **Remove Untracked Directories:** `git clean -fd`
    * **Description:** Recursively removes untracked directories in addition to standard untracked files.
* **Interactively Remove Files:** `git clean -i` (or `--interactive`)
    * **Description:** Opens an interactive prompt to review and approve the deletion of untracked files one by one.
* **Remove Ignored Files:** `git clean -fX`
    * **Description:** Removes *only* files explicitly ignored by Git (like compiled code), leaving regular untracked files alone.
