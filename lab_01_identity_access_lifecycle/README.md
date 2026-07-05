# Linux Identity & Access Lifecycle Lab

## Executive Summary
This project demonstrates competency in **Identity and Access Management (IAM)** and secure lifecycle administration within a Linux environment. As a foundational SOC task, this lab simulates the end-to-end process of managing user privileges—from initial provisioning to post-incident offboarding—ensuring the principle of least privilege is maintained throughout the identity lifecycle.

## SOC Competencies Demonstrated
*   **Identity Management:** Provisioning and de-provisioning users to manage the attack surface.
*   **Privilege & Access Control:** Utilizing `chown` and `usermod` to enforce granular access based on role requirements.
*   **System Hygiene:** Proactive removal of orphaned groups and accounts to prevent "zombie" persistence vectors.
*   **Incident Documentation:** Structured reporting of administrative actions, command validation, and post-action analysis.

## Project Context
Effective identity management is a critical pillar of a Security Operations Center (SOC). By ensuring only authorized users have access to sensitive data (like `project_r.txt`), we reduce the risk of lateral movement and insider threats.

## Tools Used
*   **Environment:** Linux Bash Shell
*   **Commands:** `useradd`, `usermod`, `chown`, `userdel`, `groupdel`
*   **Methodology:** Principles of Least Privilege, System Hardening

[View Detailed Technical Lab Report](LAB_REPORT.md)
