# ProtoConsent

<p align="center">
  <img src="https://github.com/ProtoConsent/ProtoConsent/blob/main/design/assets/logo/protoconsent_logo.png" alt="ProtoConsent logo" width="160">
</p>

<p align="center"><strong>Consent you can express, enforce and observe</strong></p>

<p align="center"><em>User-side, purpose-based consent for the web</em></p>

<p align="center">
  <img src="https://img.shields.io/badge/version-0.5.5-blue" alt="version 0.5.5">
  <img src="https://img.shields.io/github/license/ProtoConsent/ProtoConsent" alt="GPL-3.0+">
  <img src="https://img.shields.io/badge/manifest-v3-green" alt="Manifest V3">
  <img src="https://img.shields.io/badge/chromium-supported-brightgreen?logo=googlechrome&logoColor=white" alt="Chromium">
  <img src="https://img.shields.io/badge/firefox-planned-lightgrey?logo=firefox&logoColor=white" alt="Firefox planned">
</p>

ProtoConsent is a browser extension that lets you control how websites may use your data, expressed in terms of purposes (functional, analytics, ads, personalisation, third-party services, advanced tracking) rather than specific trackers or domains.

No central server, no tracking, no sharing of personal data. Preferences are enforced at the network level, per site, entirely from your browser.

<p align="center">
  <img src="https://github.com/ProtoConsent/ProtoConsent/blob/main/design/assets/screenshots/popup-profile.png" alt="ProtoConsent popup" width="360">
  &nbsp;&nbsp;
  <img src="https://github.com/ProtoConsent/ProtoConsent/blob/main/design/assets/screenshots/popup-overview-monitoring.png" alt="Overview tab dashboard" width="360">
</p>

### Highlights

- **Two operating modes**: Standalone enforces blocking directly. ProtoConsent Mode delegates to your existing blocker and adds purpose attribution - turning any ad blocker into a purpose-aware system.
- **Consent banner auto-response**: 31 CMP signatures suppress cookie popups based on your preferences - no DOM clicks, no waiting for the banner.
- **Site declarations**: websites can publish `.well-known/protoconsent.json` to declare their data practices. Open protocol with [spec](https://github.com/ProtoConsent/ProtoConsent/blob/main/design/spec/protoconsent-well-known.md), [JSON Schema](https://protoconsent.org/schema/v0.2.json), [validator](https://protoconsent.org/validate.html), and [GitHub Action](https://github.com/ProtoConsent/validate-action).
- **JavaScript SDK** (MIT) for web pages to query user preferences via `protoconsent.get('analytics')`.

> Pending review in Chrome Web Store, Edge Add-ons, and Opera Addons. In the meantime, install locally in developer mode on any Chromium-based browser.

### Repositories

| Repo | Description |
|------|-------------|
| [ProtoConsent](https://github.com/ProtoConsent/ProtoConsent) | Browser extension, SDK, protocol spec, and documentation |
| [data](https://github.com/ProtoConsent/data) | Pre-built blocklists, CMP signatures, and enhanced protection lists (CDN) |
| [demo](https://github.com/ProtoConsent/demo) | Demo site with live SDK test and `.well-known` declaration |
| [validate-action](https://github.com/ProtoConsent/validate-action) | GitHub Action + CLI to validate `.well-known/protoconsent.json` |

### Links

**Website:** [protoconsent.org](https://protoconsent.org) · **Live demo:** [demo.protoconsent.org](https://demo.protoconsent.org) · **Developer docs:** [protoconsent.org/developers](https://protoconsent.org/developers.html)
