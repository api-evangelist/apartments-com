# Apartments.com (apartments-com)

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
