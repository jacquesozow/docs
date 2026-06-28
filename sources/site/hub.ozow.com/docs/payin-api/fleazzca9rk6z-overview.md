# Source: https://hub.ozow.com/docs/payin-api/fleazzca9rk6z-overview

Overview

# Overview

**Refunds easy as that with our step-by-step guide**

The Ozow Refund API allows you to instruct us to refund any EFT payments that were paid using Ozow.

Before getting started you will require the following:

- Your Ozow merchant details:
 
 - Site code
 - Private Key
 - API Key
- That Refunds have been enabled for all sites you want to do refunds for
 

> **Refund float**
> 
> Ozow uses the funds you have loaded into your Ozow float to make refund payments.
> 
> Please see the [top up guide](https://hub.ozow.com/docs/overview/2qc4nf91ox7d1-top-up-guide) top up your float balance.

## [Overview](https://hub.ozow.com/#overview-1)

The diagram below outlines the process flow that a standard refund will follow. These steps are explained in detail in the next few sections of this guide.

## [API endpoints](https://hub.ozow.com/#api-endpoints)

Staging: [https://stagingapi.ozow.com](https://stagingapi.ozow.com)

Live: [https://api.ozow.com](https://api.ozow.com)

## [Common headers](https://hub.ozow.com/#common-headers)

All requests excluding the "get token" request require the following HTTP headers.

| Property | Type | Required | Description |
| --- | --- | --- | --- |
| Authorization | String (500) | Yes | The token generated using the get token method. eg. Authorization: Bearer \[token\] |
| Content-Type | String (50) | No | The format the response should be returned in e.g. 
Accept: application/json 
Accept: application/x-www-form-urlencoded |
| Accept | String (50) | Yes | The format the response should be returned in e.g. 
Accept: application/json 
Accept: application/xml |

[Overview](https://hub.ozow.com/#overview 'Overview') [Overview](https://hub.ozow.com/#overview-1 'Overview') [API endpoints](https://hub.ozow.com/#api-endpoints 'API endpoints') [Common headers](https://hub.ozow.com/#common-headers 'Common headers')