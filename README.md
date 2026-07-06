# Linux Administration Labs — SOC Foundations

![Linux](https://img.shields.io/badge/OS-Linux-FCC624?logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/Shell-Bash-4EAA25?logo=gnubash&logoColor=white)
![Status](https://img.shields.io/badge/Status-In%20Progress-blue)
![Cert](https://img.shields.io/badge/Google-Cybersecurity%20Certificate-4285F4?logo=google&logoColor=white)

## Overview

This repository documents hands-on Linux administration labs completed as part of the **Google Cybersecurity Professional Certificate** (Course 4: Linux and SQL), reframed through a SOC Analyst lens.

Each lab is self-contained, includes command evidence (terminal screenshots), a plain-English explanation of *why* the skill matters operationally, and a structured technical report.

This is a living repository — new labs are added as I progress through the course.

## Table of Contents

| # | Lab | Core Skill | Status |
|---|-----|-----------|--------|
| 01 | [Identity & Access Lifecycle](./lab_01_identity_access_lifecycle/) | User provisioning, privilege control, deprovisioning | ✅ Complete |
| 02 | [Linux Help & Command Discovery](./lab_02_linux_help_discovery/) | `man`, `whatis`, `apropos` — self-service troubleshooting | ✅ Complete |
| 03 | *TBD* | — | 🔜 Planned |

## Skills Demonstrated Across This Repo

| Category | Tools / Commands | SOC Relevance |
|---|---|---|
| Identity & Access Management | `useradd`, `usermod`, `userdel`, `groupdel`, `chown` | Enforcing least privilege, closing orphaned-account attack surface |
| System Documentation & Self-Help | `man`, `whatis`, `apropos` | Fast, accurate command discovery under time pressure — no guessing during triage |

## Why This Matters for a SOC Role

A large part of SOC and sysadmin-adjacent work isn't knowing every command by heart — it's knowing **how to find the right command quickly and confidently** under pressure, and applying least-privilege principles consistently. These labs build that discipline on real Linux fundamentals rather than memorized syntax.

## About Me

Second-year Bachelor of Cybersecurity student (La Trobe University) targeting a Junior SOC Analyst / Security Operations role. ISC2 CC certified. Top 3% on TryHackMe (SOC Level 1 path).
