# LOAST Ltd Privacy Notice (Training Lab)

> **Fictional company.** LOAST Ltd is a made-up organisation used in a Microsoft Entra ID identity and access management lab. This repository hosts a sample privacy notice for demonstration only. It is not a real company's privacy policy and is not legal advice.

**Live page:** `https://d-rank-developer.github.io/loast-privacy/`

## What this is

This repository contains a one-page privacy notice (`index.html`) for LOAST Ltd, a fictional London-based company. The page is published with GitHub Pages and its link is used as the **Privacy statement URL** in the LOAST Microsoft Entra tenant.

It is part of the **LOAST Enterprise Lab**, a hands-on portfolio project covering:

- Microsoft SC-300 (Identity and Access Administrator)
- Microsoft Intune endpoint management
- Governance, risk and compliance (GRC)
- A mock SOC 2 control set

## Why it exists

In Microsoft Entra ID, administrators can set a **Global privacy contact** and a **Privacy statement URL** under **Entra ID > Overview > Properties**.

When an external guest is invited to the tenant, the **Review permissions** screen shows a link to this privacy statement. If no privacy information is set, guests see a message saying the organisation has not provided links to its terms. That looks unprofessional and would be raised as a finding in an audit.

This page fixes that gap and gives evidence for the lab task **"Set tenant properties and the privacy contact"**.

## What the notice covers

| Section | Summary |
|---|---|
| 1. Who we are | LOAST Ltd as the data controller for employees, contractors and guests |
| 2. How to contact us | Privacy contact email and postal address (fictional) |
| 3. What personal data we collect | Identity, account, MFA, sign-in logs, device and guest data |
| 4. Why we use your data and our lawful basis | Account management, security, audit logs, access reviews, device management, mapped to UK GDPR lawful bases |
| 5. Who we share your data with | Microsoft (processor), IT support providers, auditors and regulators |
| 6. International transfers | UK adequacy regulations and the International Data Transfer Addendum |
| 7. How long we keep your data | Retention for staff accounts, guest accounts and logs |
| 8. Your rights | Access, correction, deletion, restriction, objection and portability |
| 9. How we protect your data | MFA, Conditional Access, least privilege and access reviews |
| 10. Complaints | Contact LOAST first, or complain to the UK ICO |
| 11. Changes to this notice | Reviewed at least once a year |

## How the page links to the Entra lab

| Entra setting | Value used in the lab |
|---|---|
| Name | LOAST Ltd |
| Technical contact | A tagged personal mailbox (kept private, not shown here) |
| Global privacy contact | A tagged personal mailbox (kept private, not shown here) |
| Privacy statement URL | This GitHub Pages link |

The public page uses `privacy@loastlab.example`, a reserved example domain, so no real email address is exposed on the internet.

## How to deploy your own copy

1. Create a **public** repository named `loast-privacy`.
2. Upload `index.html` to the root of the `main` branch.
3. Go to **Settings > Pages**.
4. Set **Source** to **Deploy from a branch**, **Branch** to `main`, folder `/ (root)`, and click **Save**.
5. After 1 to 2 minutes, open `https://<your-github-username>.github.io/loast-privacy/`.
6. Paste that link into **Entra ID > Overview > Properties > Privacy statement URL** and click **Save**.

## How to verify it in Entra

1. **Audit log:** go to **Entra ID > Monitoring & health > Audit logs** and filter **Activity** by `Update company`. The change shows who updated the tenant properties and when.
2. **Guest experience:** invite a test guest and open the invitation. The **Review permissions** screen should now link to this privacy statement.

## Repository contents

```
loast-privacy/
├── index.html   # The privacy notice page (self-contained HTML and CSS)
└── README.md    # This file
```

## Disclaimer

LOAST Ltd does not exist. This notice was written for an SC-300 identity lab and a professional portfolio. Real organisations should have their privacy notice written or reviewed by a lawyer or a data protection officer.
