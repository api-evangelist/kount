# Kount (kount)

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
