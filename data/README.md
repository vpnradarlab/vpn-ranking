# VPNRadarLab top-100 VPN ranking — open data snapshot 2026-10

The first 100 places of the [VPNRadarLab](https://vpnradarlab.com/) main ranking of 377 consumer VPNs, as published on the site on 2026-10-18 (data snapshot 2026-10-16): the overall score, six sub-scores and a set of structured, normalised facts per service.

**This is a snapshot.** Scores and places change when providers change their terms. The current ranking and the full data for each service are on the site: https://vpnradarlab.com/

| | |
|---|---|
| Version | 2026-10 |
| Data snapshot | 2026-10-16 |
| Exported | 2026-10-18 |
| Rows | 100 |
| Files | `top100.csv` (UTF-8, comma-separated, header row), `top100.json` (same rows + metadata and field list) |
| Licence | [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) |
| Update | quarterly |

## Licence and attribution

The data is licensed under the [Creative Commons Attribution 4.0 International licence](https://creativecommons.org/licenses/by/4.0/) (CC BY 4.0, full text in `LICENSE`). You may copy, share and adapt it, including commercially, **provided you credit the source with a link**:

> Source: VPNRadarLab (https://vpnradarlab.com)

Online, the words “VPNRadarLab” or the URL must link to https://vpnradarlab.com. Please also say if you changed the data.

## How to cite

> VPNRadarLab (2026). *VPNRadarLab top-100 VPN ranking*, version 2026-10 (data snapshot 2026-10-16). https://vpnradarlab.com/. Licensed under CC BY 4.0.

Machine-readable citation: `CITATION.cff`.

## How the scores work (short)

Every VPN gets six sub-scores from 0 to 10, built only from facts the provider publishes (audits, policies, apps, network, prices). The overall score is their weighted sum, also from 0 to 10. A feature counts only when the provider states it: “not stated” earns no points, which is not the same as a penalty. A red flag (stores connection IP addresses, public security incident, Chinese jurisdiction) caps the overall score at 6.0. Ties go to the service with more published data, then the smaller renewal price jump. User reviews and app-store ratings never change the score. The main ranking includes consumer VPNs with at least 60% of the data points published. Full criteria and points: https://vpnradarlab.com/methodology/

| Sub-score (column) | Name on the site | Weight |
|---|---|---:|
| `score_privacy_jurisdiction` | Privacy and jurisdiction | 30% |
| `score_security_protocols` | Security and protocols | 20% |
| `score_price_fair_terms` | Price and fair terms | 15% |
| `score_censorship_bypass` | Censorship bypass | 15% |
| `score_network_streaming` | Network and streaming | 10% |
| `score_platforms_support` | Platforms and support | 10% |

## Data dictionary

| Column | Type | Values | Description |
|---|---|---|---|
| `rank` | integer | 1–100 | Place in the VPNRadarLab main ranking (the ranking on https://vpnradarlab.com/) on the export date. |
| `name` | string | — | Service name as shown on the site. |
| `vpnradarlab_url` | string (URL) | — | The service page on vpnradarlab.com with all published data and the score breakdown. |
| `overall_score` | number | 0.00–10.00 | Overall score: weighted sum of the six sub-scores, rounded to 2 decimals as on the site. A red flag caps it at 6.0. |
| `score_privacy_jurisdiction` | number | 0.0–10.0 | Sub-score “Privacy and jurisdiction” (weight 30% of the overall score), rounded to 1 decimal as on the site. |
| `score_security_protocols` | number | 0.0–10.0 | Sub-score “Security and protocols” (weight 20% of the overall score), rounded to 1 decimal as on the site. |
| `score_price_fair_terms` | number | 0.0–10.0 | Sub-score “Price and fair terms” (weight 15% of the overall score), rounded to 1 decimal as on the site. |
| `score_censorship_bypass` | number | 0.0–10.0 | Sub-score “Censorship bypass” (weight 15% of the overall score), rounded to 1 decimal as on the site. |
| `score_network_streaming` | number | 0.0–10.0 | Sub-score “Network and streaming” (weight 10% of the overall score), rounded to 1 decimal as on the site. |
| `score_platforms_support` | number | 0.0–10.0 | Sub-score “Platforms and support” (weight 10% of the overall score), rounded to 1 decimal as on the site. |
| `segment` | string | Consumer VPN, Free / mobile app, VPN in a security suite, Gaming VPN, Decentralised (dVPN), Smart DNS | Segment (category) of the service, as on the site. |
| `jurisdiction_country` | string | country name or not_stated | Country whose law the provider operates under, as on the site. |
| `eyes_alliance` | string | 5, 9, 14, none, not_stated | Membership of the jurisdiction in the 5 / 9 / 14 Eyes surveillance alliances: 5 = Five Eyes, 9 = Nine Eyes, 14 = Fourteen Eyes, none = outside all three, not_stated = not determined. |
| `red_flag` | string | none, stores_connection_ip, public_security_incident, chinese_jurisdiction, hidden_owner | Red flag that caps the overall score at 6.0 (see the methodology). |
| `no_logs_policy` | string | yes, no, partial, not_stated | “No-logs policy” as shown on the service page. |
| `independent_no_logs_audit` | string | yes, no, partial, not_stated | “Independent no-logs audit” as shown on the service page. |
| `ram_only_servers` | string | yes, no, partial, not_stated | “RAM-only servers” as shown on the service page. |
| `kill_switch` | string | yes, no, partial, not_stated | “Kill switch” as shown on the service page. |
| `dns_leak_protection` | string | yes, no, partial, not_stated | “DNS leak protection” as shown on the service page. |
| `split_tunnelling` | string | yes, no, partial, not_stated | “Split tunnelling” as shown on the service page. |
| `wireguard` | string | yes, no, partial, not_stated | “WireGuard” as shown on the service page. |
| `openvpn` | string | yes, no, partial, not_stated | “OpenVPN” as shown on the service page. |
| `obfuscation_stealth_mode` | string | yes, no, partial, not_stated | “Obfuscation (stealth mode)” as shown on the service page. |
| `multi_hop` | string | yes, no, partial, not_stated | “Double VPN / multi-hop” as shown on the service page. |
| `open_source_apps` | string | yes, no, partial, not_stated | “Open-source apps” as shown on the service page. |
| `anonymous_signup` | string | yes, no, partial, not_stated | “Anonymous sign-up” as shown on the service page. |
| `free_plan` | string | yes, no, partial, not_stated | “Free plan” as shown on the service page. |
| `crypto_payments` | string | yes, no, partial, not_stated | “Cryptocurrency” as shown on the service page. |
| `torrenting_allowed` | string | yes, no, partial, not_stated | “Torrenting” as shown on the service page. |
| `cheapest_price_eur_month` | number or empty | — | Cheapest published price per month in EUR (longest prepaid term, converted at the snapshot exchange rate), as in the “From” column on the site. Empty: no paid price published. |
| `renewal_ratio` | number or empty | — | Renewal price per month divided by the first-term price per month (1.0 = same price at renewal). Empty: renewal price not published. |
| `refund_days` | integer or empty | — | Money-back guarantee in days; 0 = no money-back guarantee; empty = not stated. |
| `max_devices` | integer or empty | — | Simultaneous devices per subscription. Empty: unlimited (see unlimited_devices) or not stated. |
| `unlimited_devices` | string | yes, no, not_stated | yes = unlimited simultaneous devices; no = a limit is stated in max_devices. |
| `server_countries` | integer or empty | — | Number of countries with servers as published by the provider (“50+” is given as 50). Empty: not stated. |

### Value labels

- `yes` — the provider states it; `no` — the provider states it is not offered; `partial` — offered with a limitation (only some platforms, servers or countries); `not_stated` — the provider does not say. `not_stated` is **not** `no`.
- Empty numeric cells (CSV) / `null` (JSON) — not published or not applicable, as explained per column.
- Values are normalised from the provider’s own published wording with the same rules the site uses; the original wording, sources and dates of checking are on each service page.

## What is not included

Only scores and structured facts are published here. Not included: texts, comments, quotes, source links, provider website and policy URLs, change history, user reviews and ratings (Trustpilot, App Store, Google Play), search demand and traffic estimates, and places beyond 100. All of that, where we show it, is on the site.

## Report an error

If a value is wrong or outdated, tell us at https://vpnradarlab.com/report-an-error/ (name the service and the field). Corrections go to the site first and into the next snapshot.
