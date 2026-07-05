# Linux System Administration Lab: Detailed Report

**Objective:** Practice authentication and authorization lifecycle management in a Linux environment.

---

### Task 1: Add a New User
* **Action:** Created a new system account for the incoming researcher and assigned them to their primary project group.
* **Commands:** 
  * `sudo useradd researcher9`
  * `sudo usermod -g research_team researcher9`
* **Explanation:** Assigning a primary group during provisioning ensures the user has immediate, correct access to shared resources, adhering to the principle of least privilege from the start.
* **Evidence:** ![Task 1 - Add User.png](task1.png)

### Task 2: Assign File Ownership
* **Action:** Transferred ownership of a project file to the new employee to manage project assets.
* **Commands:** 
  * `sudo chown researcher9 /home/researcher2/projects/project_r.txt`
* **Explanation:** Proper file ownership is essential for accountability. By changing the owner to `researcher9`, we grant the specific user the necessary control over the file to complete their project responsibilities.
* **Evidence:** ![Task 2 - Assign Ownership.png](Task2.png)

### Task 3: Add the User to a Secondary Group
* **Action:** Extended the user's access to include a second department for cross-functional collaboration.
* **Commands:** 
  * `sudo usermod -aG sales_team researcher9`
* **Explanation:** The `-aG` flag is critical. The `-a` (append) ensures we do not overwrite existing group memberships, while `-G` adds the user to the `sales_team` as a secondary group, maintaining their access to the original research group while enabling new collaboration.
* **Evidence:** ![Task 3 - Secondary Group.png](Task3.png)

### Task 4: Delete a User
* **Action:** Removed the `researcher9` account and performed necessary system cleanup.
* **Commands:** 
  * `sudo userdel researcher9`
  * `sudo groupdel researcher9`
* **Explanation:** When a user is deleted, their dedicated primary group often remains. Manually removing this group is a security best practice to prevent "orphaned" groups from cluttering the system or potentially creating vulnerabilities.
* **Evidence:** ![Task 4. delete retired user.png](Task4.png)

---

## Reflection
This lab solidified my understanding of the user lifecycle. I encountered initial errors when attempting to modify groups that were not yet provisioned, but by analyzing the error output, I corrected the command structure. This highlighted that security administration is not just about command execution—it is about verifying the environment and following up with proper system hygiene after an account is terminated.
