# Ritele: issues and discussions

This repository is where Ritele users report bugs, request features and ask questions in public. It holds no product source code; Ritele itself is not open source.

**Ritele** draws your system architecture from OpenTelemetry traces, joins traces, metrics and logs on one live map, and tells you what gives out first when traffic grows. It is self-hosted, in one container or on Kubernetes.

- Website: https://ritele.io
- Docs: https://ritele.io/docs/
- Changelog: https://ritele.io/changelog/
- Download: https://ritele.io/download/

## Where to go

| You want to… | Go to |
| --- | --- |
| Report a bug | [New issue → Bug report](../../issues/new?template=bug_report.yml) |
| Ask for a feature | [New issue → Feature request](../../issues/new?template=feature_request.yml) |
| Ask a question or share a setup | [Discussions](../../discussions) |
| Report a security vulnerability | **Not here.** See [SECURITY.md](SECURITY.md) |
| Talk about licences, invoices or Enterprise | sales@ritele.io |

## Before you open a bug report

1. Check you're on the latest release: `docker pull ritele/ritele:latest`. Each version is listed in the [changelog](https://ritele.io/changelog/).
2. Search [existing issues](../../issues?q=is%3Aissue) first.
3. Include the version from **Settings › About** in the app (or `/healthz` on port 8080), and how you run it: Docker, or the Helm chart with embedded or external storage.

Never paste licence keys, credentials or customer data into an issue. Ritele masks recognised secrets in logs it stores, but this tracker is public.
