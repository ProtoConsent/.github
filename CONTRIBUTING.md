# Contributing to ProtoConsent

Thanks for your interest in contributing.

## Code of Conduct

This project is governed by our [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold it.

## Reporting Bugs

### Extension

Use the [Bug report](https://github.com/ProtoConsent/ProtoConsent/issues/new?template=bug_report.yml) template for issues with the popup, blocking, settings, or browser compatibility. Include your extension version (Settings > About) and browser. Paste the troubleshoot output from Settings > Support > Copy if possible.

### Filter lists and data pipeline

- [Filter issues](https://github.com/ProtoConsent/data/issues/new?template=filter_issue.yml) - wrong classification, missing domains, broken websites
- [Data pipeline bugs](https://github.com/ProtoConsent/data/issues/new?template=bug_report.yml) - list conversion, generated files, pipeline errors

## Suggesting Features

Use the [Feature request](https://github.com/ProtoConsent/ProtoConsent/issues/new?template=feature_request.yml) template. Describe the problem you want solved and any alternatives you have considered.

## Security Vulnerabilities

Do **not** open a public issue. See [SECURITY.md](SECURITY.md) for reporting instructions.

## Code Contributions

1. Fork the repository and create a branch from `main`.
2. The extension is vanilla JavaScript with no build step or npm dependencies. Load `extension/` as an unpacked extension in your browser to test.
3. Keep changes focused - one fix or feature per pull request.
4. Follow the existing code style.

## Licence

By contributing, you agree that your contributions will be licensed under the same licence as the project: [GPL-3.0-or-later](https://github.com/ProtoConsent/ProtoConsent/blob/main/LICENSE) for the extension, [MIT](https://github.com/ProtoConsent/ProtoConsent/blob/main/sdk/LICENSE) for the SDK.
