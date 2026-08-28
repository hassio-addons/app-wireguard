# Security Policy

The security of this project is taken seriously. We appreciate your efforts to
responsibly disclose any findings and will make every effort to acknowledge
your contributions.

## Supported Versions

Security updates are provided only for the latest released version of this
app. Users are strongly encouraged to keep their installations up to date.

| Version        | Supported          |
| -------------- | ------------------ |
| Latest release | :white_check_mark: |
| Older releases | :x:                |

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub issues,
discussions, or pull requests.**

Instead, report them privately through GitHub's private vulnerability
reporting:

[**Report a vulnerability**](https://github.com/hassio-addons/app-wireguard/security/advisories/new)

If for any reason you are unable to use GitHub's private vulnerability
reporting, you may also reach out to the maintainer by email at
[opensource@frenck.dev](mailto:opensource@frenck.dev).

When reporting, please include as much of the following as possible:

- A clear description of the vulnerability and its potential impact.
- Steps to reproduce, or a proof of concept.
- Affected version(s) of the app.
- Any known mitigations or workarounds.

## Disclosure Timeline

- **Acknowledgement:** you will receive an acknowledgement of your report
  within **48 hours**.
- **Initial assessment:** a triage and initial severity assessment will be
  shared within **7 days** of the acknowledgement.
- **Fix and disclosure:** valid reports are targeted for resolution and
  coordinated public disclosure within **90 days** of the initial report,
  depending on complexity and impact.

You will be kept informed throughout the process and credited in the release
notes for the fix, unless you prefer to remain anonymous.

## Out of Scope

The following are **not** considered security vulnerabilities in this project:

- Vulnerabilities in the app base image or in the Alpine packages it
  installs. These are handled continuously by
  [Renovate](https://github.com/renovatebot/renovate) and addressed through
  regular dependency updates.
- Issues only reproducible on architectures or base image versions other than
  those listed in `wireguard/build.yaml`.
- Issues in WireGuard or `wireguard-go` themselves; please report those
  directly to the [WireGuard project](https://www.wireguard.com/#contact).
- Weaknesses resulting from configuration the operator supplied themselves,
  such as custom `pre_up`, `post_up`, `pre_down` or `post_down` commands,
  hand-provided keys, or peers granted broad `allowed_ips`. The app assumes
  its own configuration is trusted.

## Scope

This security policy covers the WireGuard app published in the
[Home Assistant Community Apps repository](https://github.com/hassio-addons/repository)
and its source code in this repository.
