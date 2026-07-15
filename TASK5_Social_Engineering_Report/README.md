# Research Report: Social Engineering Attacks

## Introduction
Social engineering is the psychological manipulation of people into performing actions or giving up confidential information, credentials or access rather than exploiting software. Unlike technical exploits, social engineering targets human behavior trust, fear, urgency and curiosity instead of code making it one of the most effective and persistent attack vectors in cybersecurity reason being it bypasses firewalls and endpoint protection.

## Types of Social Engineering Attacks

### 1. Phishing
Phishing involves sending fraudulent emails, websites or messages that appear to come from a legitimate source, tricking victims into revealing sensitive information such as passwords, credit card numbers or clicking malicious links which downloads malware.

For Example:
- **Spear Phishing** – Is highly targeted at a specific individual or organisation
- **Whaling** – It is mostly targeted at high-profile executives
- **Vishing** - A method conducted through voice calls whereby individuals impersonate bank customer service departments.
- **Smishing** – A phishing method sent through SMS's commonly as fake delivery or bank alert messages.

**Real World Case Studies:**

**RSA SecurID Breach (2011):** Employees received phishing emails with a malicious Excel attachment titled "2011 Recruitment Plan." Opening it installed a backdoor, ultimately compromising RSA's SecurID authentication system and affecting client organisations worldwide.

Between 2013 and 2015, a Lithuanian attacker impersonated a hardware supplier that Google and Facebook both used, sending forged invoices and business emails that convinced employees to wire over $100 million to fraudulent accounts. The case is one of the largest documented Business Email Compromise which is a form of spear phishing incidents and led to a criminal conviction.

### 2. Pretexting
The attacker creates a fabricated scenario "pretext" to obtain information. For example, impersonating Information Technology support whether a bank official or a co-worker to gain trust and extract credentials or access.

**Real World Case Studies:**

**Twitter Bitcoin Scam (2020):** Attackers used phone based social engineering (Vishing) to trick Twitter now known as "X" employees into providing credentials to internal tools, allowing takeover of high-profile accounts (Obama, Musk and Apple) to run a Bitcoin scam which compromised more than 100 high profile accounts including those of major public figues and companies.

**How The Attacker Builds The False Scenarios:**
The attacker researches the organisation through Linkedin, press releases or previous calls to gather trustable details then constructs a scenario witha a plausible identity, urgency and authority such as claiming to be from the help desk resolving an ürgent account issue to lower the target's guard before requesting credentials or system access.

### 3. Baiting
The attacker lures victims with false promises such as free downloads, free internet access (Wireless Fidelity) and USB drives left in public areas that once accessed, they install malware or steal data.

**Different Types**

- **Physical Baiting:** Purposely leaving malicious USB drives in parking lots or hotel lobbies labeled to spark curiosity. For Example: Payroll 2024, hoping an employee plugs one into a work computer.

- **Digital Baiting:** Offers fake free software, pirated media and suspicious links that install malware.

**Real World Case Studies:**

**Ubiquiti Networks BEC Fraud (2015):** Employees were deceived through pretexting emails impersonating executives, resulting in over $46 million in fraudulent wire transfers.

The Stuxnet worm, which targeted Iranian nuclear enrichment facilities around 2010, is widely believed to have initially spread into an air gapped network through an infected USB drive a classic physical baiting vector before propagating through the industrial control systems.

## Impact on Organisations
- Financial loss such as fraud, ransom payments and regulatory fines
- Reputational damage and loss of customer trust
- Data breaches exposing sensitive customer and employee information
- Operational disruption during incident response

## Prevention Recommendations
1. **Security Awareness Training** – Provides regular, simulated phishing exercises for employees.
2. **Multi-Factor Authentication (MFA)** – This will reduce damage even if credentials are stolen.
3. **Verification Protocols** – This requires out-of-band confirmation for financialsensitive requests.
4. **Email Filtering and Anti-Phishing Tools** – It will block malicious attachments or links before they reach inboxes.
5. **Least Privilege Access** – This prevention method limits what any single compromised account can access.
6. **Incident Response Plan** – It ensures fast containment if an attack succeeds.

## Conclusion
Social engineering remains effective because it exploits human psychology rather than technical flaws. Organisations must combine technical controls with continuous employee education to build resilience against these attacks.

## References

CISA – “Avoiding Social Engineering and Phishing Attacks”: https://www.cisa.gov/news-events/news/avoiding-social-engineering-and-phishing-attacks

Verizon Data Breach Investigations Report (DBIR) – Annual Report Covering Social Engineering Trends: https://www.verizon.com/business/resources/reports/dbir/

KnowBe4 – “Social Engineering” resource hub: https://www.knowbe4.com/what-is-social-engineering

Krebs on Security – Coverage of The 2020 Twitter Bitcoin Scam: https://krebsonsecurity.com/2020/07/whos-behind-wednesdays-epic-twitter-hack/

RSA – Official Statement on The 2011 SecurID Breach: https://www.rsa.com/?s=SECURID

FBI/FTC – Business Email Compromise (BEC) Advisory, Relevant To The Ubiquiti Case: https://www.ic3.gov/CrimeInfo/BEC

Verizon Data Breach Investigations Report: https://www.verizon.com/business/resources/reports/dbir/?CMP=OOH_SMB_OTH_22222_MC_20200501_NA_NM20200079_00001

SANS Reading Room — White Papers: https://www.sans.org/white-papers/920
