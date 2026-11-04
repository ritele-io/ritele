# Security policy

## Reporting a vulnerability

Please report suspected vulnerabilities privately. **Do not open a public issue.**

- Email: **security@ritele.io**
- Or use GitHub's [private vulnerability reporting](../../security/advisories/new) on this repository.

Include the Ritele version, how it is deployed (Docker or Helm, embedded or external storage), the steps to reproduce, and the impact you expect.

## What happens next

- We acknowledge your report within 3 working days.
- We tell you whether we can reproduce it, and our plan, within 10 working days.
- We credit you in the changelog when the fix ships, unless you ask us not to.

## Supported versions

Ritele releases often. Fixes ship in the latest release, and each release is a Docker tag you can pin. Upgrade to the newest version listed in the [changelog](https://ritele.io/changelog/) before reporting.

## Verifying what you run

- Each image Ritele builds is signed with cosign and carries a CycloneDX SBOM and build provenance. The Helm chart is signed too.
- The image is distroless, with no shell or package manager.
- Licences are checked on your install; licensing never calls home.
- One daily usage ping is on by default. Set `RITELE_USAGE_PING=false` to stop it.

More detail: https://ritele.io/security/
