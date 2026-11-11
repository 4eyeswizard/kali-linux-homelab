# kali-linux-homelab
Kali installation, Linux fundamentals, GRUB troubleshooting and security experiments
# Kali Linux VirtualBox Setup & GRUB Password Recovery

**Date:** 11 November 2026  
**Environment:** Windows desktop, Oracle VirtualBox, Kali Linux 2026.3

## Objective

Deploy Kali Linux as a virtual machine for Linux fundamentals and penetration-testing practice, and document troubleshooting and security concepts encountered during installation.

## Tasks Completed

- Downloaded the Kali Linux installer ISO.
- Verified the ISO's SHA256 checksum against the official Kali Linux website.
- Enabled AMD SVM hardware virtualization in UEFI/BIOS.
- Created and configured a Kali Linux virtual machine.
- Installed Kali Linux with the Xfce desktop environment and recommended tools.
- Installed the GRUB bootloader.
- Recovered access to the Kali installation after forgetting the login credentials.

## Troubleshooting: Forgotten Linux Password

**Problem:** Unable to log into Kali Linux after installation because the account credentials were forgotten.

**Resolution:** Used GRUB's boot-entry editing capability to start a root shell, remounted the root filesystem with write access and reset the local account password.

**Outcome:** Successfully restored access without reinstalling the operating system.

## Security Lessons

1. A Linux login password does not necessarily prevent access by someone with control over an unprotected boot process.
2. Physical access and bootloader configuration are important considerations in system security.
3. Full-disk encryption can help protect data against unauthorised offline access.
4. SHA256 checksums can verify downloaded file integrity when compared against a trusted reference.

## Next Steps

- Take a clean VirtualBox snapshot.
- Practise Linux filesystem navigation and permission management.
- Continue the TryHackMe Junior Penetration Tester pathway.
- Build an isolated network for future authorised penetration-testing labs.
