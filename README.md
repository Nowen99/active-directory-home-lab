# Active Directory Home Lab

A VirtualBox lab exploring Windows domain administration, DHCP/DNS, client domain joins, and bulk user provisioning with PowerShell.

**By Noah Owen · Original lab: September 12, 2022 · Documentation migrated: November 2026**

[Full lab write-up](docs/original-article.md) · [Original Medium article](https://nowencyber.medium.com/how-to-setup-a-home-lab-running-active-directory-with-oracle-virtualbox-and-add-users-with-b05e651af52) · [Attribution](#attribution)

## Project status

This repository preserves a completed learning lab from 2022. It contains the original article and locally stored figures, with a new project overview. The environment has not been rebuilt or retested for this migration. Screenshots document the original environment; they do not establish that it is currently deployed.

## Technologies

Windows Server 2019 · Windows 10 · Oracle VirtualBox · Active Directory Domain Services · DHCP · DNS · RAS/NAT · PowerShell

## Lab workflow

1. Create a Windows Server VM with internet-facing and internal VirtualBox network adapters.
2. Install Active Directory and promote the server to a domain controller.
3. Configure RAS/NAT, DHCP, and a domain administrator account.
4. Populate the domain with over 1,000 users using the credited PowerShell script.
5. Create a Windows 10 client, join the domain, and sign in with a domain account.

## Documented results

- Domain controller and client VMs running in VirtualBox.
- DHCP and DNS configuration shown in the original screenshots.
- A populated directory and a domain-joined Windows client.
- PowerShell bulk user creation demonstrated in the original environment.

## Repository contents

| Path | Contents |
| --- | --- |
| [docs/original-article.md](docs/original-article.md) | Original article text, figures, and captions |
| [images/](images/) | Locally stored article figures |
| [docs/image-sources.json](docs/image-sources.json) | Original figure URLs and local filenames |

No VM images, original scripts, exported queries, deployment templates, or live credentials were recovered from the article. Screenshots of code are historical evidence, not executable source files.

## Attribution

The bulk user creation script used in the lab is [Josh Madakor’s AD_PS](https://github.com/joshmadakor1/AD_PS). It is linked for attribution and has not been copied into this repository.

The original article is by [Noah Owen](https://github.com/Nowen99). Referenced third-party material retains its original ownership; this migration does not claim authorship of those resources or grant a new license for them.
