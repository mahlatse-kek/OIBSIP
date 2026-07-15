# Research Report: The Importance of Patch Management

## Introduction
Patch management is the process of identifying, acquiring, testing and installing updates "patches" to software, operating systems and firmware. Patches fix security vulnerabilities, bugs and performance issues. Effective patch management is one of the most fundamental yet often neglected pillars of cybersecurity.

## What Is Patch Management?
Patch management involves:
1. **Identification** – discovering available patches from vendors.
2. **Assessment** – evaluating the severity and relevance of each patch.
3. **Testing** – verifying patches don't break existing systems.
4. **Deployment** – rolling out patches across affected systems.
5. **Verification** – confirming patches were applied successfully.

## Why Patch Management Matters
Software vulnerabilities are discovered constantly. Once a vulnerability is publicly disclosed, attackers move quickly to exploit unpatched systems often within days or hours. Patch management closes these security gaps before they can be exploited.

## Challenges and How to Overcome Them

- **Legacy Systems:** Older systems may no longer receive vendor patches.

Mitigation: Isolate them on segmented networks and apply compensating controls. For Example: Strict firewall rules until they can be retired.

- **Downtime Concerns:** Patching critical systems often requires a reboot or service interruption.

Mitigation: schedule maintenance windows and use redundant/failover systems to patch without full outages.

- **Testing Requirements:** Insufficient testing risks breaking production; excessive testing delays critical fixes.

Mitigation: Maintain a representative staging environment and set explicit, faster testing SLAs for critical/high-severity patches.

## Consequences of Failing To Patch

**WannaCry Ransomware (2017):** Exploited a known Windows SMB vulnerability called EternalBlue for which Microsoft had already released a patch two months prior. Organisations that failed to apply it including the UK's NHS, suffered massive operational disruption with an estimated 300,000+ computers infected across 150 countries.

**Equifax Data Breach (2017):** Attackers exploited a known Apache Struts vulnerability that had a patch available for months before the breach. The result was the exposure of personal data for approximately 147 million people, along with regulatory fines and reputational damage.

**General consequences of unpatched systems:**
- Increased risk of malware infection and ransomware
- Data breaches and loss of sensitive information
- Regulatory non-compliance (GDPR, HIPAA, PCI-DSS) and associated fines
- Downtime and costly incident response
- Reputational and financial damage

## Best Practices for Effective Patch Management
1. **Maintain An Asset Inventory** – you can't patch what you don't know you have.
2. **Prioritize By Risk** – patch critical/high-severity vulnerabilities first (use CVSS scores).
3. **Establish A Regular Patching Schedule** – don't wait for incidents to force action.
4. **Test Patches Before Full Deployment** – avoid breaking production systems.
5. **Automate Where Possible** – use patch management tools (WSUS, SCCM, Ansible) to reduce human error.
6. **Monitor And Verify** – confirm patches were successfully applied across all systems.
7. **Have A Rollback Plan** – in case a patch causes unexpected issues.

## Conclusion
Patch management is a simple, cost-effective defense that significantly reduces an organisation's attack surface. As shown by WannaCry and Equifax, the difference between a secure system and a costly breach is often just a delayed or missing patch. Organisations that treat patching as a continuous, prioritized process are far more resilient against cyber threats.

## References

NIST SP 800-40 Rev. 4 – “Guide to Enterprise Patch Management Planning”: https://csrc.nist.gov/pubs/sp/800/40/r4/final

CISA – Known Exploited Vulnerabilities (KEV) Catalog: https://www.cisa.gov/known-exploited-vulnerabilities-catalog

Microsoft Security Response Center – MS17-010 bulletin (the EternalBlue/WannaCry patch): https://msrc.microsoft.com/update-guide/vulnerability/CVE-2017-0144

Equifax breach report – U.S. GAO report on the 2017 breach: https://www.gao.gov/products/gao-18-559

SANS Institute – “Patch Management: Changing the Game” whitepaper: https://www.sans.org/white-papers/

MITRE CVE Program: https://www.cve.mitre.org/

National Audit Office - Official Post-Incident Reports On The WannaCry NHS impact: https://www.nao.org.uk/
