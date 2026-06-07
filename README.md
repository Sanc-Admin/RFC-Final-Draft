# RFC Final Draft — draft-vicente-oauth-apm

[![IETF Datatracker](https://img.shields.io/badge/IETF-Datatracker-blue)](https://datatracker.ietf.org/doc/draft-vicente-oauth-apm/)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](LICENSE)
[![Patent Pending](https://img.shields.io/badge/Patent-Pending-red.svg)](#ipr--patent-notice)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.20584241.svg)](https://doi.org/10.5281/zenodo.20584241)
[![ORCID](https://img.shields.io/badge/ORCID-0009--0006--6395--5308-A6CE39.svg)](https://orcid.org/0009-0006-6395-5308)


**Sanctum SecOps LLC | PATENT PENDING**

## Abstract

This repository contains the IETF Internet-Draft for the Authorization Posture Mechanism (APM) OAuth 2.0 extension, targeting the OAuth Working Group.

| Field | Value |
|---|---|
| Draft name | `draft-vicente-oauth-apm-01` |
| Working Group | IETF OAuth WG |
| Author | Brian Vicente `<bvicente@sanctumsecops.com>` |
| Status | Individual Submission |
| Date | 2026-06-05 |

## Problem Domain

OAuth 2.0 token binding exists at issuance; no per-request mechanism re-evaluates the consistency of the cert+token+device-posture triple or defines graduated least-privilege outcomes on degradation. RFC 8705 (§6.5) explicitly excludes per-request certificate re-evaluation; RFC 9449 (§11.11) explicitly excludes device posture; RFC 9470 produces only binary outcomes; OpenID CAEP is asynchronous and not in-band with individual requests. NIST SP 800-207 mandates per-request evaluation of device posture and least privilege per action — a gap the current OAuth ecosystem does not address normatively.

## Files

| File | Description |
|---|---|
| `draft-vicente-oauth-apm-01.md` | Full kramdown-rfc (mmark) I-D source |

## Related Work

- RFC 8705 (mTLS for OAuth 2.0)
- RFC 9449 (DPoP)
- RFC 9470 (OAuth Step-Up Authentication)
- RFC 9396 (Rich Authorization Requests)
- OpenID CAEP
- draft-ietf-oauth-attestation-based-client-auth-08 (2026-03-02)
- NIST SP 800-207 (Zero Trust Architecture)

## IPR Notice

PATENT PENDING — Sanctum SecOps LLC · EIN 42-2733487  
Disclosure per BCP79/RFC8179. No trade secrets disclosed.
