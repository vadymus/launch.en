---
title: Experience Cloud ID Release Notes
seo-title: Experience Cloud ID extension Release Notes in Adobe Experience Platform Launch
description: Experience Cloud ID extension Release Notes in Adobe Experience Platform Launch
seo-description: Experience Cloud ID extension Release Notes in Adobe Experience Platform Launch
---

# Experience Cloud ID Release Notes

For release notes on the Experience Cloud ID Service itself and not just the Adobe Experience Platform Launch Extension, please reference: [https://docs.adobe.com/content/help/en/id-service/using/release-notes/release-notes.html](https://docs.adobe.com/content/help/en/id-service/using/release-notes/release-notes.html)

## Oct 27, 2020

### Experience Cloud ID Extension 5.1.0

#### **Features**

* Adding `sameSiteCookie` config to specify the `SameSite` attribute of the `AMCV` cookie. This config supports the following values for `SameSite` attribute:
  * `Strict`
  * `Lax`
  * `None`

Details of these attribute values are on [web.dev](https://web.dev/samesite-cookies-explained/) and [chromium](https://www.chromium.org/updates/same-site)

## Aug 13, 2020

### Experience Cloud ID Extension 5.0.1

#### **Features**

* Updating to VisitorJS 5.0.1 patch with a fix for adding d_cf flag when the IAB consent string has changed.

## June 15, 2020

### Experience Cloud ID Extension 5.0.0

#### **Features**

* Adding support for `IAB TCF` – Transparency & Consent Framework – `Version 2.0`.

## April 13, 2020

### Experience Cloud ID Extension 4.6.0

#### **Features**

* Made `loadSSL` flag on by default. All calls to Identity Service will be on `https` by default. Customers can set it to false if they want to call Identity Services on http from their non-ssl pages.
* Updated the function used to detect Internet-Explorer (IE) version, to fix an issue reported by ESLint.
* Bug fix for a performance issue on Internet-Explorer (IE) 11 when ECID is given optIn pre-approval and updated later.

## January 22, 2020

### Experience Cloud ID Extension 4.5.2

#### **Features**

* Updated visitor.js to 4.5.2
* Visitor 4.5.1 includes a bug fix for IAB plugin for Optin
* Updated `setCustomerIDs` method to reject any empty IDs sent.

## January 7, 2020

### Experience Cloud ID Extension 4.4.2

#### **Features**

* Updated visitor.js to 4.4.2
* Improvements for `getVisitorValues` method to fetch values faster


## September 19, 2019

### Experience Cloud ID Extension 4.4.1

#### **Features**

* Updated visitor.js to 4.4.1
* Fixed a bug for get Opt-In preApprovals Input
* Renamed VIDEO_ANALYTICS to MEDIA_ANALYTICS in preOptInApprovals

  ![](/help/assets/ecid-media-analytics.png)

## July 17, 2019

### Experience Cloud ID Extension 4.4.0

#### **Features**

* Updated visitor.js to 4.4.0
* Added SHA256 hashing support for setCustomerIDs

  ![](/help/assets/ecid-setCustomerIDs-hash.png)

## May 13, 2019

### Experience Cloud ID Extension 4.3.1

#### **Features**

* Updated visitor.js to 4.3
* Added data element type for ECID as part of the Platform Launch Extension

  ![](/help/assets/ecid-data-element.png)

## April 9, 2019

### Experience Cloud ID Extension 4.2.0

#### **Features**

* Updated visitor.js to 4.2 which included support for Audience Manager IAB TCF Plug-in

## February 25, 2019

### Experience Cloud ID Extension 4.1.0

#### **Features**

* Updated visitor.js to 4.1 which updated publishDestinations per new API change. With this update the referrer information of the page can be exposed during ID - sync if desired.

## February 15, 2019

### Experience Cloud ID Extension 4.0.0

#### **Features**

* Updated visitor.js to 4.0
* Added a configuration options for the new built-in Opt-In Object. Opti-In settings can be used to suppress cookie and beacon calls of Adobe Solutions to better support regulations such as GDPR

  ![](/help/assets/ext-mcid-opt-in.png)

## March 20, 2018

### Experience Cloud ID Extension 3.1.0

#### **Features**

* Updated visitor.js to 3.1
* Adds two configuration properties: `resetBeforeVersion` and `serverState`
