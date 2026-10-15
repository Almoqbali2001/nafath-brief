Version: NAFATH-V4
Track: <one of: Software | AI | Mobile | Networking | Cybersecurity | Data>

Version: NAFATH-V4
Your track: Cybersecurity
## Overview
A secure software supply chain requires the provider to understand and protect every important component, service, and route on which its systems depend. Software configuration must be separated from source code so credentials are not accidentally exposed. AI systems need protection against attacks on both their training data and their inputs. Mobile applications should be tested against recognized security requirements before release. Internet routing protections help reduce the risk of traffic being redirected by unauthorized route announcements. Cybersecurity teams must identify vulnerable dependencies, prioritize patches, and verify that remediation works. Data transparency is equally important: a Software Bill of Materials helps teams identify components and assess exposure when a new vulnerability appears. These six fields work together to improve prevention, detection, response, and accountability across the supply chain. Log4Shell illustrates why dependency security and timely patching matter.

## Software
The Twelve-Factor App methodology says deployment-specific configuration, including service credentials and database connection details, should be stored in environment variables rather than hard-coded in source code. This separates code from settings that change between environments and reduces accidental exposure through source control. Sensitive production secrets should additionally be managed through an approved secrets manager with access controls, rotation, and auditing, rather than committed to a repository.

Resource: The Twelve-Factor App - https://12factor.net/config 
## AI
Adversarial machine-learning attacks target different stages of an AI system. Evasion attacks manipulate inputs at inference time to cause incorrect predictions. Poisoning attacks corrupt training data or the training process so the model learns harmful behavior. Privacy attacks attempt to extract sensitive information, while misuse attacks exploit a model’s capabilities for harmful purposes. Defenses require threat modelling, trusted data pipelines, robust testing, access controls, and monitoring throughout the model lifecycle.

Resource: Adversarial Machine Learning: A Taxonomy and Terminology of Attacks and Mitigations - https://csrc.nist.gov/pubs/ai/100/2/e2023/final
## Mobile
The OWASP Mobile Application Security Verification Standard (MASVS) defines security controls for mobile applications, including storage, cryptography, authentication, network communication, platform interaction, code quality, resilience, and privacy. Teams use it as a checklist of security requirements, then apply the OWASP Mobile Application Security Testing Guide (MASTG) to perform tests and collect evidence. Results help developers identify weaknesses, prioritize fixes, and verify that the app meets its intended security requirements before release.

Resource: OWASP MASVS - https://mas.owasp.org/MASVS/

## Networking
Border Gateway Protocol (BGP) route hijacking occurs when a network announces an unauthorized route for an IP prefix, potentially diverting traffic, enabling interception attempts, or causing outages. Resource Public Key Infrastructure (RPKI) lets prefix holders publish Route Origin Authorizations (ROAs), allowing networks to validate whether an autonomous system is authorized to originate a route. RPKI origin validation does not fully validate the entire AS path, encrypt traffic, or prevent every routing attack; deployment and routing policies remain essential.

Resource: BGP Origin Validation - https://www.ripe.net/manage-ips-and-asns/resource-management/rpki/bgp-origin-validation/


## Cybersecurity
Log4Shell (CVE-2021-44228) was a critical remote-code-execution vulnerability in Apache Log4j 2, a widely used Java logging library. Certain attacker-controlled log messages could trigger unsafe JNDI lookups, potentially allowing remote code execution on vulnerable systems. Its widespread use, ease of exploitation in affected configurations, and potential for severe compromise made it exceptionally serious. Organizations should identify affected applications and dependencies, upgrade to a fixed Log4j version, verify remediation, and investigate signs of compromise.

Resource: Mitigating Log4Shell and Other Log4j-Related Vulnerabilities - https://www.cisa.gov/news-events/cybersecurity-advisories/aa21-356a
## Data

## Misconception in My Track

## Open Question
