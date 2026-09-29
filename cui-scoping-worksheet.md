# CUI Scoping Worksheet: Define the Boundary Before You Score Anything

> **Created by AI Tech Pros (aitechpros.ai).** Free 90-second SPRS estimator: https://aitechpros.ai/sprs-score. The Readiness Room newsletter: https://thereadinessroom.substack.com

Your SPRS score is only valid inside the boundary your System Security Plan describes. Everything outside that boundary is out of scope; everything inside it must meet all 110 controls. Get the boundary wrong and one of two bad things happens: you scope too wide and pay to secure systems that never touch CUI, or you scope too narrow and your score is fiction because CUI actually lives somewhere you excluded.

Do this worksheet before you write your SSP or score a single control.

## Step 1: List your CUI types

CUI is unclassified information the government has marked as needing protection. Common types for small contractors: export-controlled technical data, legal or financial records tied to a contract, personally identifiable information of government personnel, and anything marked CUI in your contract documents.

| CUI type | Where the marking appears (contract clause, document banner, email label) |
|---|---|
| [Example: export-controlled drawings] | [Example: DFARS 252.204-7012 flowdown, Section C] |
| | |
| | |

If you cannot name your CUI types, stop here. Ask your prime or contracting officer what CUI you handle. Guessing is how boundaries go wrong.

## Step 2: Map where CUI lives and flows

For each location, answer: does CUI live here, pass through here, or get backed up here? Include the places contractors forget.

| Location | CUI stored? | CUI transmitted? | Notes |
|---|---|---|---|
| [Example: engineering file server] | [Yes] | [Yes] | [Engineering share] |
| Company email | | | |
| Employee laptops | | | |
| Cloud storage (OneDrive, Google Drive, Dropbox) | | | |
| Dev and test environments | | | |
| Backups and backup media | | | |
| Printers and multifunction devices | | | |
| Mobile phones and tablets | | | |
| Removable media (USB drives) | | | |
| Subcontractor systems | | | |
| Personal devices (if used for work) | | | |
| | | | |

## Step 3: Draw the boundary

Your CUI boundary is the set of people, systems, and locations that store, process, or transmit CUI. Write it as a plain-English paragraph first, then as a list.

**Boundary statement:** [Example: "The CUI boundary includes the engineering file server, the eight company laptops used by engineering staff, company email, and the encrypted backup NAS. It excludes the guest Wi-Fi network, the accounting workstation, and personal devices, which are prohibited from handling CUI by policy POL-014."]

**In scope:**

-
-
-

**Explicitly out of scope (with justification):**

- [Example: guest Wi-Fi, segmented with no route to CUI systems]
-
-

## The five scoping mistakes small contractors make

### 1. Scoping the whole network instead of segmenting

Putting every workstation, printer, and IoT device in scope because "it is easier." It is not easier; it multiplies your assessment surface and your remediation bill. Segment CUI onto the smallest set of systems you can defend, and document the segmentation.

### 2. Forgetting email and backups

CUI in an inbox is CUI in scope. CUI on a backup NAS is CUI in scope. Contractors routinely scope the file server and forget that the same data flows through email and lands on backups. If it appeared in Step 2, it belongs in the boundary.

### 3. Treating the SSP boundary as the network boundary

Your SSP describes the system that handles CUI, not your entire company network. But the reverse error is just as common: describing a tidy boundary in the SSP while CUI actually flows across systems you left out. The boundary must match reality, not the org chart.

### 4. Ignoring flowdown to subcontractors and primes

If you receive CUI from a prime or pass it to a sub, those flows are part of your scoping problem. Your boundary ends where theirs begins, but you need to know where that line is and document it.

### 5. Allowing CUI on unmanaged or personal devices

"Just this once" on a personal laptop puts that laptop in scope. Either prohibit it with enforced policy and technical controls, or scope it in and secure it. There is no third option.

## When you are done

Transfer your boundary statement into Section 2 of `ssp-template.md`. Every control implementation statement you write after that is written against this boundary. If the boundary changes (new contract, new system, new CUI type), update the worksheet, then the SSP, then your score, in that order.
