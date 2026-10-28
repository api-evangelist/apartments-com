# Apartments.com

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Apartments.com is the largest United States rental-listings marketplace, owned by CoStar Group since its 2014 acquisition and operated from Arlington, Virginia as the anchor of the Apartments.com Network — a group of consumer rental sites that also includes ApartmentFinder.com, ApartmentHomeLiving.com, ForRent.com, ForRentUniversity.com, WestsideRentals.com, Apartamentos.com, After55.com and CorporateHousing.com. It sits on the demand side of the US residential value chain as an Internet Listing Service (ILS): apartment owners and property managers buy advertising, and their inventory, availability, pricing, media, concessions and fee data flows in from property management systems (Yardi, RealPage, Entrata, MRI, AppFolio, ResMan, Rent Manager, Funnel, EliseAI and others) rather than from any public API, while leads flow back out to the advertiser's CRM. Its API posture is closed. Apartments.com publishes no developer portal, no OpenAPI or OData $metadata contract, no SDK, no webhooks and no Postman collection; developer.apartments.com, developers.apartments.com and docs.apartments.com do not resolve in DNS, and api.apartments.com resolves only to the same Akamai edge that returns HTTP 403 Access Denied to every non-browser request, including robots.txt. The one documented machine-to-machine seam is the Digital Feeds Program — an approval-and-contract path in which an approved third-party feed vendor syndicates a paying advertiser's listings into Apartments.com over FTP using an XML listings feed whose specification guide is available only on request to Feeds@apartments.com. A second inbound seam lets licensed agents opt in to rental-listing syndication through their own MLS (Bright MLS, ARMLS, REcolorado, OneKey MLS, SmartMLS, NorthstarMLS, MLS PIN, Garden State MLS, New Jersey MLS and Aspen Glenwood MLS are documented), which requires MLS membership. On RESO, the honest reading is absence rather than "certified but unreachable": Apartments.com does not appear anywhere in the RESO certificates list, and its own property-manager help centre returns zero results for "RESO". It is a consumer of MLS rental feeds, not a certified RESO endpoint, and no unlicensed open dataset is published.

**Areas:** Real Estate · United States · Rentals · Property Listings · Multifamily · Internet Listing Service · Listings Syndication · Property Management · MLS · PropTech · CoStar Group

## Apartments.com on APIs.io

Everything profiled for Apartments.com is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/apartments-com/](https://apis.io/providers/apartments-com/)** — or go straight to one of the APIs or properties below.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Apartments Com Authentication](https://apis.io/security/apartments-com/apartments-com-authentication/)
- [Apartments Com Domain Security](https://apis.io/security/apartments-com/apartments-com-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.apartments.com)
- [Documentation](https://propertyhelp.apartments.com/collection/1044-ils-integrations)
- [Sign up](https://www.apartments.com/rental-manager/list-property-for-rent)
- [Support](https://propertyhelp.apartments.com/)
- [Terms of service](https://www.apartments.com/grow/about/terms-of-service)
- [Privacy policy](https://www.apartments.com/grow/about/privacy-notice)
- [GitHub](https://github.com/AptsCom)

## API Evangelist rating

**Kin Score 17.6** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 48.2 |
| Contract quality | 0.0 |
| Contract governance | 18.2 |
| Operational transparency | 2.6 |
| Developer ergonomics | 14.3 |
| Access clarity | 34.2 |

**Agent readiness 0.0** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | — |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 18.6** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/apartments-com/](https://apis.io/providers/apartments-com/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Apartments.com: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/apartments-com/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
