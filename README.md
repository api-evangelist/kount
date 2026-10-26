# Kount (kount)

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

Kount is a Boise, Idaho-based fraud prevention and chargeback management platform, now operating as part of Equifax. Kount combines AI-driven risk scoring, device fingerprinting, identity intelligence, and a multi-tenant global data network to help merchants, payment processors, and digital businesses stop payment fraud, account takeover, and chargebacks while reducing false positives. The Kount 360 platform offers Payments Fraud, Account Takeover Protection, Chargeback Management, and Identity Trust services exposed through REST APIs, mobile SDKs, a JavaScript Data Collector, and e-commerce platform plugins.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/kount/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Fraud Prevention, Fraud Detection, Chargebacks, Payments, Identity, Risk Scoring, Device Intelligence, Account Takeover

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Kount Payments Fraud API

The Payments Fraud API is the core REST endpoint of the Kount 360 platform for AI-driven digital fraud prevention. Merchants submit order, payment, customer, and device session data, and receive a real-time risk decision (Approve, Decline, Review) along with a risk score and reason codes. Authentication is via OAuth 2.0 bearer tokens. A sandbox is available at api-sandbox.kount.com and production at api.kount.com.

**Human URL:** [https://developer.kount.com/hc/en-us/articles/14474979202068-Payments-Fraud-v2-0-Integration-Guide](https://developer.kount.com/hc/en-us/articles/14474979202068-Payments-Fraud-v2-0-Integration-Guide)

#### Tags:

 - Payments Fraud, Risk Scoring, Decisioning

#### Properties

- [Documentation](https://developer.kount.com/hc/en-us/articles/14474979202068-Payments-Fraud-v2-0-Integration-Guide)
- [APIReference](https://developer.kount.com/hc/en-us/articles/40305795712916-Get-Orders-API-Specification)
- [Authentication](https://developer.kount.com/hc/en-us/sections/4410851086356-Integration)

### Kount Risk Inquiry Service (RIS) API

The Risk Inquiry Service (RIS) is Kount's legacy RESTful API for transaction risk evaluation. RIS joins device data from the JavaScript Data Collector with merchant-supplied order data, scores each transaction, and returns Approve, Decline, or Review responses. Transactions continue to be evaluated and re-scored for up to fourteen days. Sub-resources cover VIP lists (card, email, device, address, payment, gift, UDF), order detail, refund/chargeback (RFCB), and 3DS transaction tagging. Test endpoint api.test.kount.net/rpc/v1 and production api.kount.net/rpc/v1.

**Human URL:** [https://developer.kount.com/hc/en-us/articles/4411554840980-RESTful-Endpoint-API-Specification-and-Error-Codes](https://developer.kount.com/hc/en-us/articles/4411554840980-RESTful-Endpoint-API-Specification-and-Error-Codes)

#### Tags:

 - Risk Inquiry, Transactions, VIP Lists, Chargebacks

#### Properties

- [Documentation](https://developer.kount.com/hc/en-us/articles/4411554840980-RESTful-Endpoint-API-Specification-and-Error-Codes)
- [APIReference](https://api.kount.net/rpc/list.html)
- [SDK - RIS Java SDK](https://github.com/Kount/kount-ris-java-sdk)
- [SDK - RIS PHP SDK](https://github.com/Kount/kount-ris-php-sdk)
- [SDK - RIS Python SDK](https://github.com/Kount/kount-ris-python-sdk)
- [SDK - RIS .NET SDK](https://github.com/Kount/kount-ris-dotnet-sdk)

### Kount Data Collector

The Kount Data Collector is a client-side JavaScript and mobile SDK component that gathers device fingerprinting and behavioral session data — including device characteristics, browser attributes, IP geolocation, and proxy detection — and ties it to a session identifier that is later submitted to RIS or the Payments Fraud API. The Data Collector is delivered as a hosted JavaScript snippet, an Android SDK, and an iOS SDK (both Objective-C/Swift bridge and pure-Swift variants).

**Human URL:** [https://developer.kount.com/hc/en-us](https://developer.kount.com/hc/en-us)

#### Tags:

 - Device Intelligence, Fingerprinting, Session

#### Properties

- [Documentation](https://developer.kount.com/hc/en-us)
- [SDK - Web (JavaScript) SDK](https://github.com/Kount/kount-web-sdk)
- [SDK - Android SDK](https://github.com/Kount/kount-android-sdk)
- [SDK - iOS SDK (Objective-C)](https://github.com/Kount/kount-ios-sdk)
- [SDK - iOS SDK (Swift)](https://github.com/Kount/kount-swift-ios-sdk)

## Common Properties

- [Website](https://kount.com/)
- [Portal](https://developer.kount.com/)
- [Developer](https://developer.kount.com/)
- [Documentation](https://developer.kount.com/hc/en-us)
- [GettingStarted](https://developer.kount.com/hc/en-us/sections/4410851086356-Integration)
- [GitHubOrganization](https://github.com/Kount)
- [Support](https://support.kount.com/)
- [LinkedIn](https://www.linkedin.com/company/kount)
- [ParentCompany - Equifax (Parent Company)](https://www.equifax.com/business/identity-fraud/)
- [SDK - RIS Java SDK](https://github.com/Kount/kount-ris-java-sdk)
- [SDK - RIS PHP SDK](https://github.com/Kount/kount-ris-php-sdk)
- [SDK - RIS Python SDK](https://github.com/Kount/kount-ris-python-sdk)
- [SDK - RIS .NET SDK](https://github.com/Kount/kount-ris-dotnet-sdk)
- [SDK - Android Data Collector SDK](https://github.com/Kount/kount-android-sdk)
- [SDK - iOS Data Collector SDK (Objective-C)](https://github.com/Kount/kount-ios-sdk)
- [SDK - iOS Data Collector SDK (Swift)](https://github.com/Kount/kount-swift-ios-sdk)
- [SDK - Web (JavaScript) Data Collector SDK](https://github.com/Kount/kount-web-sdk)
- [Integrations - Magento 2 Plugin (Kount 360)](https://github.com/Kount/magento2-kount-360)
- [Integrations - Salesforce Commerce Cloud Link](https://github.com/Kount/sfcc_link)
- [Sample - Sample E-Commerce Web App](https://github.com/Kount/kount-sample-web-app)

## Features

| Name | Description |
|------|-------------|
| AI-Driven Risk Scoring | Machine learning models score each transaction in real time and return Approve, Decline, or Review decisions with reason codes. |
| Device Fingerprinting | JavaScript and mobile Data Collectors capture device, browser, network, and behavioral signals tied to a session identifier. |
| Identity Trust Network | A multi-tenant global data network correlates personas across merchants to identify trusted customers and known fraudsters. |
| Chargeback Management | Refund/Chargeback (RFCB) reporting plus dispute response workflows reduce chargeback losses and recover revenue. |
| Account Takeover Protection | Login and account-change risk scoring detects credential stuffing, session hijacking, and synthetic account creation. |
| VIP Lists | Merchant-managed allow/deny lists for cards, emails, devices, addresses, payment instruments, gift cards, and custom UDFs. |
| 3-D Secure Orchestration | 3DS transaction tagging API supports step-up authentication for stronger customer authentication where required. |
| Custom Decisioning Rules | Merchants can layer business rules on top of the model score via the Agent Web Console. |
| Mobile SDKs | Native Android and iOS SDKs (Objective-C and Swift) for in-app device data collection. |
| E-Commerce Platform Plugins | Out-of-the-box integrations for Magento 2, Shopify, Salesforce Commerce Cloud, and Miva. |

## Use Cases

| Name | Description |
|------|-------------|
| Card-Not-Present Payment Fraud | Score e-commerce CNP transactions for stolen-card and BIN-attack fraud before authorization. |
| Chargeback Reduction | Pre-authorization screening and post-transaction chargeback tagging to reduce chargeback ratios. |
| Account Takeover Defense | Score login and password-reset events to block credential-stuffing and ATO attempts. |
| New Account Fraud | Screen account-creation events for synthetic identities and bot signups. |
| Digital Goods and Gift Card Fraud | High-velocity digital goods and gift-card flows benefit from device + persona network signals. |
| Marketplace Trust | Two-sided marketplaces use Kount to vet both buyers and sellers. |
| Promo Abuse and Policy Abuse | Detect coupon stacking, refund abuse, and other policy-abuse patterns via custom rules and UDFs. |

## Integrations

| Name | Description |
|------|-------------|
| Magento 2 | Official Magento 2 plugin for the Kount 360 platform. |
| Shopify | Shopify app integration for Kount risk decisioning. |
| Salesforce Commerce Cloud | SFCC Link cartridge for Kount integration. |
| Miva | Miva e-commerce platform integration documented in Miva developer docs. |
| Equifax | Parent-company integration with Equifax identity and credit data services. |

## Solutions

| Name | Description |
|------|-------------|
| Kount 360 | Unified fraud prevention platform combining Payments Fraud, Account Takeover, and Chargeback Management on a single AI model. |
| Payments Fraud | Real-time CNP transaction screening for merchants and payment processors. |
| Account Takeover Protection | Login and account-event risk scoring to block credential abuse. |
| Chargeback Management | Pre-transaction prevention plus post-transaction dispute response workflows. |
| Identity Trust Global Network | Cross-merchant persona data network underlying all Kount decisions. |

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
