# MMN.CC — Cryptocurrency Fraud Threat Intelligence Case Study

**Case ID:** MMN-2026-001  
**Investigation period:** November 2026  
**Classification:** Suspected cryptocurrency fraud / private-key harvesting  
**Methodology:** Passive OSINT and limited manual observation  
**Disclosure status:** Pending confirmation

> This case study documents suspicious activity observed during
> an unsolicited cryptocurrency solicitation. It does not establish
> criminal attribution, confirmed theft, or a successful takedown.

## Executive Summary

In November 2026, the investigator received an unsolicited TikTok
message claiming access to a cryptocurrency account containing
approximately 5,384,624.80 USDT.

The sender supplied credentials and directed the recipient to:

https://www.mmn.cc/index/user/index.html

The website presented a login interface. Using only the credentials
provided in the unsolicited message, the investigator observed
requests for a cryptocurrency deposit, external trading-account
linking, a wallet address, and a field explicitly labelled
"Private Key".

No personal credentials, wallet secrets, or funds were submitted.

These observations are consistent with suspected advance-fee
cryptocurrency fraud and possible private-key harvesting.

## Investigation Objectives

- Document the suspicious solicitation
- Identify publicly visible infrastructure indicators
- Assess potential risks to cryptocurrency users
- Preserve evidence with integrity checks
- Prepare responsible abuse reports
- Publish sanitized findings for defensive awareness

## Technical Findings

| Indicator | Observed value |
|---|---|
| Domain | mmn.cc |
| Reported URL | https://www.mmn.cc/index/user/index.html |
| Resolved IPv4 | 45.195.197.201 |
| Registrar | Gname.com Pte. Ltd. |
| Domain creation | 2011-03-02 |
| WHOIS network assignee | Zillion Network Inc |
| Network prefix | 45.195.197.0/24 |
| Route objects | AS139613, AS54801 |
| Reverse DNS | No PTR response observed |
| MX records | No MX response observed |

The network information reflects registration and routing database
records at the time of investigation. It does not prove that the
listed organizations operate or knowingly support the website.

The domain's age and WHOIS update dates are not independently
evidence of malicious activity.

## Observed Suspicious Behaviors

1. Unsolicited social-media message promising access to substantial
   cryptocurrency funds.
2. Login credentials supplied by the sender.
3. Cryptocurrency deposit requested.
4. External trading-account linking requested.
5. Wallet address requested.
6. A field explicitly labelled "Private Key" requested.

The private-key request is particularly concerning because disclosure
of a real cryptocurrency private key may enable unauthorized control
of associated funds.

The website's backend behavior, actual collection of submitted keys,
and any resulting financial theft have not been verified.

## Potential Victim Impact

- Loss of cryptocurrency through requested deposits
- Compromise of wallets if private keys are submitted
- Compromise of linked trading accounts
- Exposure of personal or financial information

These are potential impacts, not confirmed victim outcomes.

## Investigation Methodology

See [methodology/INVESTIGATION.md](methodology/INVESTIGATION.md).

## Indicators

See [indicators/iocs.csv](indicators/iocs.csv).

Indicators are provided for investigation and correlation.
They are not proof that every service on the associated IP is malicious.

## Responsible Disclosure

See [disclosure/TIMELINE.md](disclosure/TIMELINE.md).

No abuse submission or enforcement outcome should be described as
completed without a corresponding confirmation.

## Evidence Handling

Original screenshots, supplied login credentials, personal
information, and raw private evidence are excluded from this
public repository.

Evidence files should be retained privately, with SHA-256 hashes
and collection timestamps.

## Scope and Limitations

This was not a penetration test.

No exploitation, vulnerability scanning, brute forcing, automated
interaction, or attempted service disruption was performed.

The investigator used supplied credentials for limited manual
observation. No authorization from the website operator was obtained
for security testing.

The findings are based on firsthand observations and passive
WHOIS/DNS records, without independent verification of the site's
backend behavior or attribution.

## Ethical Statement

This project exists for cybersecurity education, fraud awareness,
defensive threat intelligence, and responsible disclosure.

It does not endorse unauthorized access, retaliation, or disruption
of infrastructure.

## Skills Demonstrated

- OSINT
- DNS investigation
- WHOIS analysis
- Infrastructure attribution limitations
- Threat intelligence documentation
- Cryptocurrency fraud awareness
- Evidence integrity
- Responsible disclosure
- Technical reporting

## Author

Independent Cybersecurity Researcher

## Disclaimer

All findings represent observations at the documented time.
Infrastructure, DNS records, and website behavior may change.
