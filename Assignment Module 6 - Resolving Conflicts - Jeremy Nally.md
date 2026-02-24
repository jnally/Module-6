# Assignment Module 6 - Resolving Conflicts - Jeremy Nally

## To Begin Resolution
Regardless of the scenario, start with these steps:
1. Open the conflicted file in a text editor.
2. Locate the conflict markers:
   * `<<<<<<< HEAD` (marks the beginning of the local changes)
   * `=======` (separates the local changes from the incoming changes)
   * `>>>>>>> aca5fc717753bbebc5486c9cb741b33100ce3943` (marks the end of the incoming changes)
3. Edit the file to reflect the final desired state by removing the conflict markers and any unwanted lines.

---

## To only keep "- Sleep"
To keep the local changes and reject the remote changes, do the following in the text editor:
1. Delete the `<<<<<<< HEAD` marker line.
2. Leave the `- Sleep` line intact.
3. Delete the `=======` separator line.
4. Delete the incoming change line `- Gym`.
5. Delete the `>>>>>>> aca5fc717753bbebc5486c9cb741b33100ce3943` marker line.

**Final File State:**

    - Eat
    - Read
    - Sleep

---

## To only keep "- Gym"
To reject the local changes and accept the incoming remote change, do the following in the text editor:
1. Delete the `<<<<<<< HEAD` marker line.
2. Delete the local change line `- Sleep`.
3. Delete the `=======` separator line.
4. Leave the `- Gym` line intact.
5. Delete the `>>>>>>> aca5fc717753bbebc5486c9cb741b33100ce3943` marker line.

**Final File State:**

    - Eat
    - Read
    - Gym

---

## To keep both "- Sleep" and "- Gym"
To keep both changes, do the following steps in the text editor:
1. Delete the `<<<<<<< HEAD` marker line.
2. Leave the `- Sleep` line intact.
3. Delete the `=======` separator line.
4. Leave the `- Gym` line intact.
5. Delete the `>>>>>>> aca5fc717753bbebc5486c9cb741b33100ce3943` marker line.

**Final File State:**

    - Eat
    - Read
    - Sleep
    - Gym

---

## Finalize with Git
Once the edits to the file have been made, finalize the merge in Git with these steps:
1. **Save** the file in the text editor.
2. Open a terminal and stage the resolved file using the command: `git add <filename>`
3. Complete the merge by committing the changes: `git commit -m "Resolve merge conflict"`
4. Push the resolved commit back to the shared repository: `git push`
