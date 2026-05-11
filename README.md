# Windows Baseline Configuration Snapshot Collector
## CYB 125 Final Project — Part 1: Project Plan

**Student name:** Caileb Church
**Date:** May 11, 2026

---

## About this Project

This script will collect information from the operating system including the Windows Registry, performance counters, and various command line utilities relating to system configuration. The data will then be analyzed, catagorized, and labelled in groups. A .json file will be produced with a hierarchical list of configurations such as the source, configuration name, and current value.

---

## Approach

I will gather data from three categories of sources:

- Windows Registry (read with the `winreg` Python module)
- Performance counters (sampled with the `typeperf` command)
- Command-line utilities (invoked from Python with `subprocess`)

---

## Data Dictionary

All data will be stored in a dictionary with each value listed as follows:

{
  "snapshot_metadata": {
  },
  "system_identity": {
  },
  "hardware_profile": {
    "cpu": {
    },
    "memory": {
    },
    "bios": {
    },
    "system": {
    },
    "logical_disks": []
  },
  "network_configuration": {
    "primary_dns_suffix": ,
    "adapters": []
  },
  "listening_ports": [],
  "local_user_accounts": {
    "current_user": ,
    "users": [],
    "administrators_group_members": []
  },
  "password_policy": {},
  "auto_start_services": [],
  "running_processes": [],
  "installed_software": [],
  "installed_hotfixes": [],
  "persistence_locations": {
    "hklm_run": [],
    "hkcu_run": [],
    "hklm_run_once": [],
    "hkcu_run_once": [],
    "all_users_startup_folder": {},
    "current_user_startup_folder": {}
  },
  "scheduled_tasks": [],
  "security_posture": {
    "firewall": {
      "domain_profile": {},
      "private_profile": {},
      "public_profile": {}
    },
    "windows_defender": {},
    "uac": {},
    "bitlocker": {},
  "performance_snapshot": {},
    "disk_system_volume": {},
    "process_count":
  },
  "network_shares": []
}

---

## Configuration Areas

### 1. snapshot_metadata
Information regarding properties of a snapshot.

### 2. system_identity
Information regarding your system's authentication and identity

### 3. hardware_profile
Information regarding the hardware components installed into your system

### 4. network_configuration
Information regarding how your network is configured

### 5. listening_ports
Information regarding the ports your computer is monitoring for information/requests over your network

### 6. local_user_accounts
Accounts on your system

### 7. password_policy
Current password rules

### 8. auto_start_services
Services that start automatically without user input

### 9. running_processes
Currently running processes

### 10. installed_software
Software installed on your system

### 11. installed_hotfixes
Hotfixes installed on your system

### 12. persistence_locations
Areas where software is automatically started upon system boot

### 13. scheduled_tasks
Tasks scheduled to run on your system

### 14. security_posture
Your systems security profile

### 15. performance_snapshot
Your systems performance in a set monitoring window

### 16. network_shares
Your systems shared files on your network

---

## Strategy

I plan to use AI in the following way....

Three prompts I plan to use:

1. What is an efficient way to do _
2. How can I rewrite this to make readability better
3. Any general question really

I will use AI mostly as a way to save time and mental thinking power. A good way to ensure that the AI's code works properly is to test and manually read it over. I expect that it would be helpful when doing tedious typing tasks like building large dictionaries or lists. I guess I could also ask it general questions like google.
---

## Milestones

The project is structured around eight milestones, each one designed to produce a working JSON file with an additional section implemented. The milestone structure isn't just a grading convenience, it's a deliberate AI-collaboration pattern. 

When students use AI well, they treat it like a pair programmer: they bring it small, well-scoped problems, ask it to explain things rather than just produce things, and verify its answers against an authoritative source (the textbook, the official Python docs, or their own running code). The output is code they understand and could rewrite from scratch.

The eight-milestone structure exists to force responsible AI usage. Each milestone is small enough that you can hold the whole thing in your head. Each milestone has a specific Python concept attached to it, so you know what you're supposed to be learning. Each milestone has a suggested AI prompt that asks for explanation, not code.

Your goal is not to finish the project as fast as possible. Your goal is to finish the project understanding what you built. Those are different goals. The milestone structure pushes you toward the second one.



---

## Notes for the Instructor
among us susy