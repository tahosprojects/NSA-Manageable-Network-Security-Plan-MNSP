# NSA Manageable Network Security Plan (MNSP)

Applied the NSA's Manageable Network Plan, an 8-milestone framework for turning an unmanaged network into a documented, defensible, and maintainable one, to a home network environment. Covers network discovery, segmentation, protocol hardening, access control, patch management, and security documentation end to end.

**Stack:** Nmap · Kali Linux · Windows · VMware (isolated lab segment)

## Methodology

The assessment followed all 8 MNSP milestones in order:

1. **Prepare:** established a centralized, version-controlled documentation repository with change tracking, encrypted backups, and offline hard-copy availability for critical procedures.
2. **Map:** used Nmap host discovery to enumerate active devices, build a device inventory (role, status, approval), and diagram the physical and logical network path from gateway to endpoint.
3. **Protect:** defined network enclaves (a general-use segment and an isolated VMware lab segment), identified high-value assets and choke points, and documented containment, encryption, and incident response procedures.
4. **Reach:** eliminated clear-text administrative protocols (HTTP, Telnet, FTP) in favor of HTTPS-only management, disabled remote administration by default, and required VPN for any remote access.
5. **Control:** enforced least-privilege, non-administrative accounts for daily use, separated administrative credentials from standard accounts, and restricted network access to approved, reviewed devices.
6. **Manage (Patch Management):** implemented automatic OS and firmware updates, tracked non-Microsoft software updates, and identified and avoided end-of-life hardware and software.
7. **Manage (Baseline Management):** defined a device security baseline, an approved-applications allowlist, endpoint antivirus protection, and unique, password-manager-issued credentials across accounts.
8. **Document:** maintained administrative process documentation, system rebuild procedures, and backup/recovery runbooks sufficient for another administrator to execute without verbal instruction.

## Key Findings

Applying a structured framework to an unmanaged network surfaced real, prioritizable gaps rather than a generic checklist. The completed assessment identified specific open items around network segmentation depth, intrusion detection coverage, remote-access tooling, and centralized identity management, each mapped back to the milestone it falls under and each with a documented remediation path.

## Skills Demonstrated

Network discovery and asset inventory with Nmap, network segmentation and enclave design, protocol and administrative-access hardening, least-privilege access control, patch and baseline management, and security documentation aligned to a recognized framework (NSA MNSP) and referencing NIST SP 800-41, 800-34, and 800-61.

## A Note on Scope

This assessment was performed against a real, in-use network rather than a disposable lab environment. Specific IP addressing, device inventory, and identified security gaps are intentionally omitted from this public write-up. Publishing a live network's exact topology and open weaknesses is itself a security mistake, and recognizing that distinction is part of the assessment.
