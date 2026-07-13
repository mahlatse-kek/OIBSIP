# Research Report: The Importance of Patch Management

## Introduction
Patch management is the process of identifying, acquiring, testing and installing updates "patches" to software, operating systems and firmware. Patches fix security vulnerabilities, bugs and performance issues. Effective patch management is one of the most fundamental yet often neglected pillars of cybersecurity.

## What Is Patch Management?
Patch management involves:
1. **Identification** – discovering available patches from vendors
2. **Assessment** – evaluating the severity and relevance of each patch
3. **Testing** – verifying patches don't break existing systems
4. **Deployment** – rolling out patches across affected systems
5. **Verification** – confirming patches were applied successfully

## Why Patch Management Matters
Software vulnerabilities are discovered constantly. Once a vulnerability is publicly disclosed, attackers move quickly to exploit unpatched systems often within days or hours. Patch management closes these security gaps before they can be exploited.

## Consequences of Failing to Patch

**WannaCry Ransomware (2017):** Exploited a known Windows SMB vulnerability (EternalBlue) for which Microsoft had already released a patch two months prior. Organizations that failed to apply it including the UK's NHS, suffered massive operational disruption with an estimated 300,000+ computers infected across 150 countries.

**Equifax Data Breach (2017):** Attackers exploited a known Apache Struts vulnerability that had a patch available for months before the breach. The result was the exposure of personal data for approximately 147 million people, along with regulatory fines and reputational damage.

**General consequences of unpatched systems:**
- Increased risk of malware infection and ransomware
- Data breaches and loss of sensitive information
- Regulatory non-compliance (GDPR, HIPAA, PCI-DSS) and associated fines
- Downtime and costly incident response
- Reputational and financial damage

## Best Practices for Effective Patch Management
1. **Maintain an asset inventory** – you can't patch what you don't know you have
2. **Prioritize by risk** – patch critical/high-severity vulnerabilities first (use CVSS scores)
3. **Establish a regular patching schedule** – don't wait for incidents to force action
4. **Test patches before full deployment** – avoid breaking production systems
5. **Automate where possible** – use patch management tools (WSUS, SCCM, Ansible) to reduce human error
6. **Monitor and verify** – confirm patches were successfully applied across all systems
7. **Have a rollback plan** – in case a patch causes unexpected issues

## Conclusion
Patch management is a simple, cost-effective defense that significantly reduces an organisation's attack surface. As shown by WannaCry and Equifax, the difference between a secure system and a costly breach is often just a delayed or missing patch. Organisations that treat patching as a continuous, prioritized process are far more resilient against cyber threats.

