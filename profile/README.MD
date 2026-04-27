# ProtoConsent

<p align="center">
  <img src="https://github.com/ProtoConsent/ProtoConsent/blob/main/design/assets/logo/protoconsent_logo.png" alt="ProtoConsent logo" width="160">
</p>

<p align="center"><strong>Consent you can express, enforce and observe</strong></p>

<p align="center"><em>User-side, purpose-based consent for the web</em></p>

ProtoConsent organizes privacy around **purposes** instead of individual trackers or domains. The project has two main outputs: a browser extension for end users and purpose-based blocklists for any tool.

No central server, no tracking, no sharing of personal data.

---

### Browser extension

<p align="center">
  <img src="https://img.shields.io/badge/version-0.5.6-blue" alt="version 0.5.6">
  <img src="https://img.shields.io/github/license/ProtoConsent/ProtoConsent" alt="GPL-3.0+">
  <img src="https://img.shields.io/badge/manifest-v3-green" alt="Manifest V3">
  <img src="https://img.shields.io/badge/chromium-supported-brightgreen?logo=googlechrome&logoColor=white" alt="Chromium">
  <img src="https://img.shields.io/badge/firefox-planned-lightgrey?logo=firefox&logoColor=white" alt="Firefox planned">
</p>

A personal consent control panel that lives in the browser. Not a full ad blocker, not a CMP - it can coexist with existing blockers and consent tools.

- **Two operating modes**: Blocking enforces purpose-based blocking directly. Monitoring delegates to your existing blocker and adds purpose attribution and signal observability.
- **Consent banner auto-response**: 31 CMP signatures suppress cookie popups based on your preferences - no DOM clicks, no waiting for the banner.
- **Per-site profiles and purpose toggles**: assign a trust level per site and refine individual purposes.
- **Site declarations**: websites can publish `.well-known/protoconsent.json` to declare their data practices. Open protocol with [spec](https://github.com/ProtoConsent/ProtoConsent/blob/main/design/spec/protoconsent-well-known.md), [JSON Schema](https://protoconsent.org/schema/v0.2.json), [validator](https://protoconsent.org/validate.html), and [GitHub Action](https://github.com/ProtoConsent/validate-action).
- **JavaScript SDK** (MIT) for web pages to query user preferences via `protoconsent.get('analytics')`.

<p align="center">
  <img src="https://github.com/ProtoConsent/ProtoConsent/blob/main/design/assets/screenshots/popup-profile-dark.png" alt="ProtoConsent popup" width="360">
  &nbsp;&nbsp;
  <img src="https://github.com/ProtoConsent/ProtoConsent/blob/main/design/assets/screenshots/popup-overview-monitoring.png" alt="Overview tab dashboard" width="360">
</p>

<p align="center">
  <a href="https://microsoftedge.microsoft.com/addons/detail/protoconsent/djghmcahfjgmeiocpgkdgengofconfoo"><img src="https://github.com/ProtoConsent/ProtoConsent/blob/main/design/assets/icons/microsoft-edge-add-ons-badge.png" alt="Get it from Microsoft Edge" height="56"></a>
  &nbsp;
  <img src="https://github.com/ProtoConsent/ProtoConsent/blob/main/design/assets/icons/chrome.svg" alt="Chrome" height="18"> <em>Chrome Web Store - in review</em>
  &nbsp;&nbsp;
  <img src="https://github.com/ProtoConsent/ProtoConsent/blob/main/design/assets/icons/opera.svg" alt="Opera" height="18"> <em>Opera Addons - in review</em>
</p>

---

### Purpose-based blocklists

<p align="center">
  <img src="https://img.shields.io/badge/domains-250K+-blue" alt="250K+ domains">
  <img src="https://img.shields.io/badge/purposes-6-green" alt="6 purposes">
  <img src="https://img.shields.io/badge/formats-5-orange" alt="5 formats">
  <img src="https://img.shields.io/badge/updated-daily-brightgreen" alt="Updated daily">
</p>

Tracker blocklists organized by data-processing purpose, available in 5 formats. Use them with any ad blocker, DNS sinkhole, or browser extension - no ProtoConsent extension required.

| Format | Compatible with |
|--------|-----------------|
| ABP | uBlock Origin, Adblock Plus, Ghostery |
| AdGuard | AdGuard browser extension |
| Hosts | Pi-hole, AdGuard Home, /etc/hosts |
| Domains | NextDNS, ControlD, RethinkDNS |
| JSON | MV3 browser extensions, custom tools |

Six purpose lists: **Ads**, **Analytics**, **Personalization**, **Third Parties**, **Advanced Tracking**, **Security**.

See the [data repo](https://github.com/ProtoConsent/data) for download links and quick start URLs.

---

### Repositories

| Repo | Description |
|------|-------------|
| [ProtoConsent](https://github.com/ProtoConsent/ProtoConsent) | Browser extension, SDK, protocol spec, and documentation |
| [data](https://github.com/ProtoConsent/data) | Purpose-based tracker blocklists in 5 formats - 250K+ domains, updated daily |
| [protoconsent.org](https://github.com/ProtoConsent/protoconsent.org) | Project website, blog, validator, generator, and directory |
| [demo](https://github.com/ProtoConsent/demo) | Demo site with live SDK test and `.well-known` declaration |
| [validate-action](https://github.com/ProtoConsent/validate-action) | GitHub Action + CLI to validate `.well-known/protoconsent.json` |

### Links

**Website:** [protoconsent.org](https://protoconsent.org) · **Live demo:** [demo.protoconsent.org](https://demo.protoconsent.org) · **Developer docs:** [protoconsent.org/developers](https://protoconsent.org/developers.html)
