# Apartments.com (apartments-com)

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

Apartments.com is the largest United States rental-listings marketplace, owned by CoStar Group since its 2014 acquisition and operated from Arlington, Virginia as the anchor of the Apartments.com Network. It sits on the demand side of the US residential value chain as an Internet Listing Service (ILS): apartment owners and property managers buy advertising, and their inventory flows in from property management systems rather than from any public API. Its API posture is closed — no developer portal, no OpenAPI or OData `$metadata` contract, no SDK, no webhooks, and no RESO certification.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/apartments-com/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/apartments-com/refs/heads/main/apis.yml)

## Tags

- Real Estate
- United States
- Rentals
- Property Listings
- Multifamily
- Internet Listing Service
- Listings Syndication
- Property Management
- MLS
- PropTech
- CoStar Group

## Timestamps

- **Created:** 2026-07-26
- **Modified:** 2026-07-26

## APIs

None. Apartments.com publishes no public, documented developer API.

Every candidate developer host is either absent from DNS (`developer.apartments.com`, `developers.apartments.com`, `docs.apartments.com`, `partners.apartments.com`, `feeds.apartments.com`, `data.apartments.com`) or served by the same Akamai edge that returns `HTTP 403 Access Denied` to non-browser clients (`www.apartments.com`, `api.apartments.com`) — including `/robots.txt`, `/openapi.json`, `/swagger.json`, `/api-docs`, `/$metadata`, and `/.well-known/openid-configuration`.

## RESO Posture

**Not certified.** Apartments.com does not appear in the [RESO certificates list](https://www.reso.org/certificates/) (578 certificate entries checked on 2026-07-26; zero matches for "CoStar", "Apartments" or "Homes.com"), and its own property-manager help centre returns **zero** articles for a search on "RESO".

Apartments.com is a downstream **consumer** of MLS rental listings, not a certified RESO Web API endpoint. Licensed agents opt in to Apartments.com syndication from inside their own MLS; ten MLSs are documented individually — Bright MLS, ARMLS, REcolorado, OneKey MLS, SmartMLS, Northstar MLS, MLS Property Information Network, Garden State MLS, New Jersey MLS, and Aspen Glenwood MLS. Data travels *into* Apartments.com. Nothing comes back out to a developer.

## Access Gate

`partner-only`. There is no path by which an independent developer obtains credentials.

1. **Digital Feeds Program** — be a paying Apartments.com advertiser, apply by emailing `Feeds@apartments.com`, and route data through an approved third-party feed vendor. The listings-feed XML guide is not published; it is supplied on request. Documented transport is FTP (server name, login, password).
2. **MLS syndication opt-in** — hold membership in a participating MLS and toggle Apartments.com syndication inside that MLS's own system.

Neither issues an API key. Neither returns data to the caller. No open, unlicensed dataset is published.

## Auth Model

None published. Feed authentication is out-of-band FTP username/password issued between the feed vendor and Apartments.com. Advertiser and renter accounts use ordinary web session logins.

## Webhooks, SDKs, Postman

None. Lead delivery into an advertiser's CRM is configured inside the PMS/CRM vendor's own product (Yardi, Rent Manager, WelcomeHome, EliseAI), not through any Apartments.com-published contract.

## Common Properties

- [Website](https://www.apartments.com)
- [About](https://www.apartments.com/about)
- [Parent — CoStar Group](https://www.costargroup.com/about-us/brands/apartmentscom)
- [Property Owner and Manager Help Center](https://propertyhelp.apartments.com/)
- [ILS Integrations](https://propertyhelp.apartments.com/collection/1044-ils-integrations)
- [MLS Integrations](https://propertyhelp.apartments.com/collection/1201-mls-integrations)
- [What is a Feed?](https://propertyhelp.apartments.com/article/439-what-is-a-feed)
- [Listings Feed Program](https://ecom.apartments.com/advertise/resources/listings-feed-program)
- [Digital Feeds Program](https://www.apartments.com/advertise/advfeeds)
- [Renter Help Center](https://renterhelp.apartments.com/)
- [Rental Manager](https://www.apartments.com/rental-manager)
- [GitHub Organization](https://github.com/AptsCom)
- [LinkedIn](https://www.linkedin.com/company/apartments-com)
- [Twitter](https://x.com/apartmentscom)
- [YouTube](https://www.youtube.com/@apartmentscom)
- [Instagram](https://www.instagram.com/apartmentscom/)

## Review

See [review.yml](review.yml) for every URL probed, its HTTP status, the RESO posture block, and the verbatim quotes behind the access-gate classification.

## Maintainers

- Kin Lane — kin@apievangelist.com
