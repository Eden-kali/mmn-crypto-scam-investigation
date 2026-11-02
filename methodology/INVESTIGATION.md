# Investigation Methodology

## Phase 1 — Initial Detection

Source: unsolicited TikTok direct message.

The message claimed access to a cryptocurrency account holding
approximately 5.38 million USDT and supplied a website URL
and login credentials.

The original screenshot should be retained privately.

## Phase 2 — Limited Manual Observation

The investigator visited the supplied website and used the
credentials provided in the message.

Observed features included:

- Login interface
- Cryptocurrency deposit request
- External trading-account linking
- Wallet address request
- Explicit "Private Key" field

No personal wallet information or funds were submitted.

No further account interaction is recommended.

## Phase 3 — Passive Domain Reconnaissance

Commands used:

    whois mmn.cc
    dig mmn.cc A +short
    dig mmn.cc NS +short
    dig mmn.cc MX +short
    dig www.mmn.cc A +short

The observed IPv4 address was:

    45.195.197.201

## Phase 4 — Network Registration Research

Commands used:

    whois 45.195.197.201
    dig -x 45.195.197.201 +short

AFRINIC WHOIS identified a network assignment associated
with Zillion Network Inc.

Two route objects were returned, listing AS139613 and AS54801.

These records do not independently establish the currently
originating ASN or the physical location of the server.

## Phase 5 — Risk Assessment

Assessment: High concern for suspected cryptocurrency fraud.

Potential impact of actual private-key disclosure: Critical.

Confidence:

- High: firsthand observation of a "Private Key" field
- High: observed DNS and WHOIS output at collection time
- Moderate: suspected fraud mechanism
- Unverified: actual theft, backend collection, and operator identity

## Phase 6 — Responsible Disclosure

Prepare reports for the registrar and relevant defensive
reporting services.

Preserve confirmation numbers and response dates privately.

Do not publish confidential correspondence without permission.

## Investigation Boundaries

No vulnerability scans, exploitation, credential attacks,
wallet connections, private-key submissions, or service
disruption were performed.

The limited login observation is documented transparently;
it should not be represented as authorized penetration testing.
