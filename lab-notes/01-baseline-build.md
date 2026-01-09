# Active Directory Baseline Build

## Purpose

The purpose of this phase was to build a functional Active Directory environment exactly as described in the source walkthrough, without introducing hardening, auditing, or security controls.

This baseline serves as a control state for later security-focused observations.

---

## Lab Scope and Constraints

- Single Domain Controller
- Single Windows client
- DNS and DHCP enabled
- Bulk user creation via PowerShell
- Default configuration settings only

Out of scope for this phase:
- Hardening
- Advanced auditing
- Detection tooling
- Exploitation testing

---

## Environment Overview

| Component        | Description                     |
|------------------|---------------------------------|
| Domain Controller| Windows Server (AD DS, DNS)     |
| Client           | Windows workstation (Domain-joined) |
| Identity         | Domain users created via script |

---

## Build Summary

The environment was built following the walkthrough with no deviations.

Key outcomes:
- Domain services were functional
- Client successfully joined the domain
- Domain users were able to authenticate
- No security configuration was modified

---

## Security Observations (Baseline)

At this stage, no security controls were added.

Initial observations:
- Authentication works with minimal friction
- Authorization is largely implicit
- Logging and visibility were not addressed during setup

These observations were intentionally left unexplored until later phases.

---

## Why This Baseline Matters

Establishing an untouched baseline is critical for understanding:

- What Active Directory considers “normal”
- What risk exists before misconfiguration or abuse
- What defenders can and cannot observe by default

This baseline will be used for comparison in later security extensions.
