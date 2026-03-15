---
title: Introduction to CVE's
description: Today I wanted to learn more about CVEs.
categories: ["CVE"]
tags: ["CVE"]
date: 2026-03-14
---

Today I decided that I would learn more about CVEs. Even if you don’t know much about cybersecurity or computers in general, you have more than likely heard of a CVE. This is because they affect everyone. One of the most well-known CVEs is Log4Shell (CVE-2021-44228). I remember hearing a lot about this vulnerability, even some friends who didn’t know too much about computers were discussing it with me. Although knowing about Log4Shell doesn’t necessarily mean you understand what a CVE is.

## What is a CVE?

CVE stands for **Common Vulnerabilities and Exposures**. The name is pretty telling on what a CVE is, `vulnerabilities and exposures` although one thing that did confuse me was `common`. Even though I would say some vulnerabilities are common/widespread, I wouldn't say all of them are. Some can be very uncommon. After researching this, the best explanation I could come up with was that it more refers to them being common in the way that they were identified and cataloged. Which I believe this does make since. CVEs have a lot they share in common with how they are cataloged. CVEs are commonly kept in databases hosted for the public to view. There are quite a few CVE databases you can find online. When looking through all of the CVE records, you will notice all that they share in common. Each CVE record has a `CVE Identifier (CVE ID)`. You will also notice that each CVE record has something called the `Common Vulnerability Scoring System (CVSS)`.

### CVE Identifier
CVE Identifier, also called CVE ID, is used to identify an individual CVE. An example of this would be CVE-2021-44228, which is the CVE for the Log4Shell vulnerability. This means there will not be any duplicate CVE IDs.

### Common Vulnerability Scoring System
 Common Vulnerability Scoring System, also called CVSS, is used in scoring. In a CVSS, you can note that each CVE record is listed with a score, severity, and vector. You may also see that a CVE record has more than one CVSS. This is because of CVSS versioning. Each CVSS version differs in how a vulnerability is scored. This mean between the different versions, you will notice the final scores are different. 

#### Score
The score is ranged 0 to 10. 10 is the highest score a CVE record can have. Something I wondered was if a score can actually be scored as a 0. It turns out it can. A 0 would basically mean that it wouldn't score in any of the metrics.

#### Severity
Severity is based on the score. This means if it gets a 1.2 score than the severity couldn't be high it would have to be low. The exact score to severity table would be

| Severity  | Score      |
| --------  | ---------- |
| None      | 0.0        |
| Low       | 0.1 - 3.9  |
| Medium    | 4.0 - 6.9  |
| High      | 7.0 - 8.9  |
| Critical  | 9.0 - 10.0 |

#### Vector
The vector is a text string that represents the scoring metrics used to score the CVE record. It will start off with the version of CVSS used. Then go into the actual metrics used. : is kind of used as an = in the vector. An example would be `AV:N` which would mean Attack Vector = Network. Each metric is then separated by /. There are some mandatory metrics used but not all are mandatory. 

### How are CVEs created?
The first step in how CVEs are created is a vulnerability is found. Once someone finds a vulnerability it is then reported. The best way is to report the vulnerability to a CVE program partner. Once it is reported the `CVE Numbering Authority (CNA)` will then assign a CVE ID to the report to make it a CVE record. 

## Conclusion
I enjoyed researching this subject. Before today, I knew a little about CVEs in the instance that I would know a certain vulnerability and know there would be a CVE ID. I also knew about the severity. It was interesting learning about the scoring and the vector of a CVE record. While researching, I found a ton of good resources I can use to find and research CVEs. This will definitely help me in future write-ups. I feel much better about my knowledge of CVEs and hope to build upon this as well. 

## Interesting facts I found while researching
> * CVE was originally called `Common Vulnerability Enumeration`
> * CVE identifiers used to start with `CAN-` before they would be approved. 