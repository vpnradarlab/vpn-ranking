# VPNRadarLab — VPN ranking methodology

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23457598.svg)](https://doi.org/10.5281/zenodo.23457598)

**Website: [vpnradarlab.com](https://vpnradarlab.com/)** · Live methodology page: [vpnradarlab.com/methodology/](https://vpnradarlab.com/methodology/)

How every VPN on VPNRadarLab gets its score: six sub-scores built from published facts, fixed weights, the criteria and points behind each one, and the rules for missing data, red flags and ties. This file restates the methodology page; if the two ever differ, the live page is the reference.

## The score in one paragraph

Every VPN gets six sub-scores from 0 to 10, built only from facts the provider publishes: independent audits, privacy policies, apps, protocols, network and prices (including renewal prices). The overall score is their weighted sum, also from 0 to 10. A red flag caps it at 6.0. There are no affiliate links, no paid placements and no sponsored rankings on the site.

## Six sub-scores and their weights

| Sub-score | Weight | Criteria | Points for a full score |
|---|---|---|---|
| Privacy and jurisdiction | 30% | 12 | 15 |
| Security and protocols | 20% | 12 | 14 |
| Price and fair terms | 15% | 10 | 12 |
| Censorship bypass | 15% | 12 | 10.5 |
| Network and streaming | 10% | 8 | 8.5 |
| Platforms and support | 10% | 10 | 10.5 |

In each sub-score the points add up and are divided by the points needed for a full score; the result is capped between 0 and 10.

### Privacy and jurisdiction (30%)

| Criterion | Points |
|---|---|
| No-logs policy | +2 |
| Independent no-logs audit | +3 |
| No logs confirmed in court | +1 |
| Policy says connection IPs are not stored | +1.5 |
| Policy says session times are not stored | +1 |
| Jurisdiction and surveillance alliances: outside 14 Eyes 1, 14 Eyes 0.4, 9 Eyes 0.3, 5 Eyes 0, not stated 0 | +2 |
| Warrant canary | +1 |
| Transparency report | +1 |
| Sign-up without email | +1.5 |
| Account number sign-up | +0.5 |
| Stores connection IP (penalty) | −3 |
| Public incident (penalty) | −2 |

### Security and protocols (20%)

| Criterion | Points |
|---|---|
| Kill switch | +2 |
| DNS leak protection | +1.5 |
| WireGuard or an own modern protocol | +1.5 |
| RAM-only servers | +1 |
| Post-quantum encryption | +1 |
| Perfect forward secrecy | +0.5 |
| Security audit | +2 |
| Open-source clients | +1.5 |
| 2FA | +1 |
| Multi-hop | +1 |
| Bug bounty | +1 |
| Only PPTP / L2TP (penalty) | −2 |

### Price and fair terms (15%)

| Criterion | Points |
|---|---|
| Cheapest price per month: percentile among consumer VPNs, cheaper scores higher; no published price scores 0 | +2.5 |
| Free plan | +1.5 |
| Free trial | +1 |
| Trial without a card | +1 |
| Refund window, in proportion up to 30 days | +1.5 |
| Devices at once, in proportion up to 10 | +1 |
| Crypto payments | +1 |
| Cash payments | +0.5 |
| Fair terms, each: refunds on monthly plans, pro-rata refunds, auto-renewal off by default, cancelling without support, a renewal reminder, plans shorter than a month | +0.5 each |
| Renewal price jump (penalty): renewal price per month over the cheapest 12+ month plan, from 1.3× up to the full penalty at 3× | −2 |

### Censorship bypass (15%)

| Criterion | Points |
|---|---|
| Stealth / obfuscation | +2 |
| VLESS / Reality | +1.5 |
| Trojan | +1 |
| Hysteria2 | +1 |
| Shadowsocks | +1 |
| AmneziaWG | +1 |
| obfs4 | +0.5 |
| TUIC | +0.5 |
| NaiveProxy | +0.5 |
| Mirrors or Telegram channel | +0.5 |
| VoIP in the UAE (claimed) | +0.5 |
| Manual configs | +0.5 |

### Network and streaming (10%)

| Criterion | Points |
|---|---|
| Number of server countries: percentile among consumer VPNs (log scale) | +2 |
| Number of servers: percentile among consumer VPNs (log scale) | +1.5 |
| 10 Gbps servers | +1 |
| Dedicated IP | +0.5 |
| Port forwarding | +0.5 |
| MENA locations | +0.5 |
| Streaming claims: Netflix, BBC iPlayer, Disney+, Prime Video; two or more gives the full points | +1.5 |
| Torrenting allowed | +1 |

### Platforms and support (10%)

| Criterion | Points |
|---|---|
| Apps for Windows, macOS, Linux, iOS and Android, in proportion of the five | +3 |
| Routers | +1 |
| An app for Android TV, Apple TV or Fire TV | +0.5 |
| Browser extensions | +0.5 |
| Split tunneling | +1 |
| Ad / tracker blocker | +1 |
| 24/7 live chat | +2 |
| Live chat | +0.5 |
| Support on Telegram | +0.5 |
| Status page | +0.5 |

## Rules

- **Normalisation.** Each sub-score is the sum of its points divided by the points needed for a full score, capped between 0 and 1 and shown out of 10. Counts such as countries and servers are compared as percentiles among consumer VPNs on a log scale, so a provider with thousands of servers does not drown everyone else. Price is a percentile too: cheaper scores higher.
- **"Not disclosed" scores zero — it is not the same as "no".** A feature counts only when the provider states it. If a policy does not say whether something is collected or offered, it earns no points, which is not a penalty. Penalties apply only to facts the provider states: keeping connection IPs, session times, a public security incident, PPTP or L2TP only, a large renewal price jump.
- **Claimed vs confirmed.** Claims and confirmations are separate criteria: a no-logs policy earns 2 points, an independent no-logs audit 3 more, a no-logs claim confirmed in court 1 more, a security audit 2. Data a provider sends us counts only after it has been checked against what the provider publishes.
- **Red flags and the 6.0 cap.** A VPN that stores connection IP addresses, had a public security incident or is under Chinese jurisdiction cannot score above 6.0, however strong the rest is. The reason is shown on its page.
- **Ties.** When two VPNs have the same score, the one with more published data ranks higher, then the one with the smaller renewal price jump.
- **Who is in the main ranking.** Only consumer VPNs (six segments: consumer, free and mobile apps, VPNs in security suites, gaming VPNs, decentralised VPNs, Smart DNS) with at least 60% of the data points published. Business, self-hosted, router, provider, browser and white-label services are scored the same way and have their own catalogue pages.

## Weight presets on topic pages

Some rankings weigh the sub-score that matters for that topic more. The chosen sub-score gets the preset weight and the other five share the rest in their usual proportions. Red flags still apply.

| Preset | Used on | Privacy | Security | Price | Censorship | Network | Platforms |
|---|---|---|---|---|---|---|---|
| Led by privacy and jurisdiction | Anonymity · Jurisdictions | 45% | 16% | 12% | 12% | 8% | 8% |
| Led by security and protocols | Security | 22% | 40% | 11% | 11% | 8% | 8% |
| Led by price and fair terms | Price and payment | 21% | 14% | 40% | 11% | 7% | 7% |
| Led by censorship bypass | Protocols · Travel and restrictions | 21% | 14% | 11% | 40% | 7% | 7% |
| Led by network and streaming | Use cases · Servers by country | 20% | 13% | 10% | 10% | 40% | 7% |
| Led by ecosystem | Platforms · Support · Languages | 22% | 14% | 11% | 11% | 7% | 35% |
| Base weights | Main ranking · Segments (except business) and other | 30% | 20% | 15% | 15% | 10% | 10% |

## What is not measured, and why

- **No speed tests.** A speed test measures one server, from one place, at one moment, over one internet provider; the result says more about the route than about the VPN. The score uses what stays true for everyone: protocols, server network, published terms.
- **No blocking tests.** Whether a VPN works in a restricted country changes week to week and differs by city and mobile operator. Where streaming or access in restricted countries is mentioned, it is the provider's own claim and labelled as such.
- **User reviews do not change the score.** Store and review-site ratings are shown on service pages, smoothed, but they never change the score, directly or indirectly.

## Data

The [`data/`](data/) folder holds an open snapshot of the **top 100 of the VPNRadarLab main ranking** (2026-10):

- [`data/top100.csv`](data/top100.csv) and [`data/top100.json`](data/top100.json) — place, overall score, the six sub-scores, segment,
  jurisdiction, 5/9/14 Eyes, red flag, 15 key features as `yes` / `no` / `partial` / `not_stated`, and a few numbers (cheapest price per
  month in EUR, renewal ratio, refund days, devices, server countries);
- [`data/README.md`](data/README.md) — what each field means, the scales and what is left out (texts, sources, user reviews, store ratings,
  traffic estimates are not included).

It is a snapshot, updated quarterly; current scores are on [vpnradarlab.com](https://vpnradarlab.com/). Each release (`v2026-10` and later)
has the files as a zip archive.

The 2026-10 snapshot is also archived on Zenodo with a DOI: [10.5281/zenodo.23457598](https://doi.org/10.5281/zenodo.23457598) (record: https://zenodo.org/records/23457598).

**Licence:** the data is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) ([`data/LICENSE`](data/LICENSE)).
Credit it with a link: **Source: VPNRadarLab (https://vpnradarlab.com)**.

**How to cite:** VPNRadarLab (2026). *VPNRadarLab top-100 VPN ranking*, version 2026-10 [Data set]. Zenodo. https://doi.org/10.5281/zenodo.23457598. https://vpnradarlab.com/. CC BY 4.0.
Machine-readable: [`CITATION.cff`](CITATION.cff).

Found a wrong value? Report it at https://vpnradarlab.com/report-an-error/.

## Found an error?

Report it on the site: [vpnradarlab.com/report-an-error/](https://vpnradarlab.com/report-an-error/).

## License

The text of this repository is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE). Please credit "VPNRadarLab (vpnradarlab.com)".
