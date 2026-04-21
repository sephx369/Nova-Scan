# Nova Scan

> Free WordPress malware scanner. Four detection engines. Catches what signature scanners miss.

[![Download](https://img.shields.io/badge/Download-Free-38bdf8?style=for-the-badge)](https://novaheaven.io/en/novascan)
[![License](https://img.shields.io/badge/License-Proprietary-f59e0b?style=for-the-badge)](https://novaheaven.io/en/novascan)
[![WordPress](https://img.shields.io/badge/WordPress-5.0%2B-21759b?style=for-the-badge&logo=wordpress&logoColor=white)](https://wordpress.org)
[![PHP](https://img.shields.io/badge/PHP-7.4%2B-777bb4?style=for-the-badge&logo=php&logoColor=white)](https://php.net)

Nova Scan is a free WordPress malware scanner built by a solo developer in Tennessee. It runs four detection engines (PHP, JavaScript, database, firewall) and a learning detection engine that catches obfuscated, polymorphic, and novel malware the signature-based scanners miss.

**Free forever. No paid tier. No upsells inside scan results.** Hyper Nova and the other Nova Heaven plugins fund Nova Scan staying free.

## Why another scanner

WordPress malware scanners are expensive and mostly pattern-matchers. Wordfence Premium is $119/yr, Sucuri is $199/yr, MalCare is $99/yr. They all rely on signature databases, which means they miss anything the vendor hasn't cataloged yet.

Nova Scan takes a different approach: it reads the structure of your files and understands what the code is *doing*, not just matching strings. Obfuscated payloads, variable-name shuffling, base64/eval chains, packed droppers — the engine follows them.

| | Nova Scan | Wordfence Premium | Sucuri | Patchstack |
|---|---|---|---|---|
| Price | Free | $119/yr | $199/yr | $49/yr |
| Learning detection engine | Yes | No | No | No |
| Shared-hosting compatible | Yes | Partial | Partial | Yes |
| Setup time | ~2 minutes | ~15 minutes | ~30 minutes | ~5 minutes |
| False positive rate | Near-zero | Medium | Medium | Low |

Detailed comparisons:
- [Nova Scan vs Wordfence](https://novaheaven.io/en/novascan-vs-wordfence)
- [Nova Scan vs Sucuri](https://novaheaven.io/en/novascan-vs-sucuri)
- [Nova Scan vs Patchstack](https://novaheaven.io/en/novascan-vs-patchstack)

## Install

1. Create a free account at [novaheaven.io](https://novaheaven.io) (Google, GitHub, or email).
2. Install [Nova Core](https://novaheaven.io/en/novacore) (required framework, also free).
3. Install Nova Scan.
4. Run your first scan.

Works on any WordPress install, including shared hosting (Hostinger, SiteGround, Bluehost). No shell access needed.

## What Nova Scan does

- Full-site malware scanning across PHP, JavaScript, database, and firewall layers
- Learning detection engine that tracks novel malware patterns across the user base
- Auto-quarantine for high-confidence findings
- Three-pass triage → analysis → verdict to eliminate false positives
- Live web application firewall with virtual patching for known CVEs
- Detailed finding reports with file paths, line numbers, confidence scores
- One-click cleanup for confirmed malware
- Privacy-first telemetry (opt-in, hashed, minimal)

## What this repo is

This is the public-facing repo for Nova Scan. It's where you can:

- **File bug reports** — open an issue if you hit a false positive, a crash, or a feature gap
- **Request detection improvements** — paste a hash or structural description (no live malware content please)
- **Track releases** — tagged releases with changelog
- **Read docs** — pointers to the full documentation

Nova Scan itself is proprietary and distributed as a signed plugin zip through the authenticated Nova Heaven distribution system. The source code is not in this repository.

If you're looking for an open-source variant, see **[novascan-lite](https://wordpress.org/plugins/novascan-lite/)** on the WordPress.org plugin directory (GPLv2, stripped feature set).

## Reporting a security vulnerability

Do not file security issues in the public tracker. Email **security@novaheaven.io** directly or use the contact form at [novaheaven.io/en/contact](https://novaheaven.io/en/contact). See [SECURITY.md](./SECURITY.md) for the full disclosure policy.

## Links

- **Website** — [novaheaven.io](https://novaheaven.io)
- **Docs (Codex)** — [novaheaven.io/en/codex](https://novaheaven.io/en/codex)
- **Blog (Nova Pulse)** — [novaheaven.io/en/novapulse](https://novaheaven.io/en/novapulse)
- **RSS** — [novaheaven.io/feed](https://novaheaven.io/feed/)
- **Mastodon** — [@novaheaven@novaheaven.io](https://novaheaven.io/@novaheaven)
- **Telegram community** — [t.me/nova_heaven](https://t.me/nova_heaven)
- **Wikidata** — [Q139409241 (Nova Scan)](https://www.wikidata.org/wiki/Q139409241) · [Q139409209 (Nova Heaven)](https://www.wikidata.org/wiki/Q139409209)

## Built by

[@sephx369](https://github.com/sephx369) · [@sephx@mastodon.social](https://mastodon.social/@sephx) · [Wikidata Q139409139](https://www.wikidata.org/wiki/Q139409139)

Solo developer, Tennessee, 25 years full-stack. Nova Heaven is the product of building what I needed and couldn't afford.

~SephX
