# Linux System Administration Lab

**Objective:** Manage user lifecycles and file permissions in a Linux Bash shell to ensure secure access control.

## Workflow & Evidence

### Task 1: Add a new user
* **Action:** Created the `researcher9` user account and assigned them to the `research_team` primary group.
* **Evidence:** ![Task 1 - Add User.png](Task 1 - Add User.png)

### Task 2: Assign file ownership
* **Action:** Transferred ownership of `/home/researcher2/projects/project_r.txt` to `researcher9`.
* **Evidence:** ![Task 2 - Assign Ownership.png](Task 2 - Assign Ownership.png)

### Task 3: Add the user to a secondary group
* **Action:** Added `researcher9` to the `sales_team` supplementary group using `usermod -aG`.
* **Evidence:** ![Task 3 - Secondary Group.png](Task 3 - Secondary Group.png)

### Task 4: Delete a user
* **Action:** Removed the `researcher9` account and performed cleanup of the associated group to maintain system hygiene.
* **Evidence:** ![Task 4. delete retired user.png](Task 4. delete retired user.png)

## Reflection
This lab highlighted that security isn't just about setting permissions—it’s about the full lifecycle of an identity. I learned that manual cleanup of orphaned groups (using `groupdel`) is a critical step in reducing the attack surface after a user has been offboarded.
