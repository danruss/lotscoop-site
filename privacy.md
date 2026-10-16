---
title: LotScoop Privacy Policy
permalink: /privacy/
---

# LotScoop Privacy Policy

**Effective date:** October 16, 2026

This policy explains what the LotScoop browser extension ("LotScoop", "the
extension", "we") does with information. The short version: LotScoop has no
servers of its own and no analytics. It looks up public land and hazard data
for the home you are viewing, and it keeps a small amount of data in your own
browser. If you start the free trial or buy LotScoop, the payment service
ExtensionPay and its card processor Stripe handle your email address and
payment details.

## Where the extension runs

LotScoop's panel runs only on pages of www.zillow.com. The extension also
loads ExtensionPay's small script on extensionpay.com pages, so it can tell
when you have confirmed a trial or finished a payment there. It does not read,
change, or monitor any other website you visit, and it does not read your
browsing history, bookmarks, tabs, or other browser data.

## What the extension reads

On those pages, LotScoop reads information about the property you select (an
open listing, a map marker's pop-up card, or a listing card you rest the
pointer on):

- the property's street address and map coordinates,
- its list price, and
- the tax history shown on an open listing (annual tax amounts and assessed
  values).

It does not read your name, email address, saved homes, messages, sign-in
details, or anything about your Zillow account.

## What is sent to other services, and why

To show land and hazard information, the extension sends the **selected
property's address and/or coordinates** — never information about you — to
these free public services:

| Service | Address | What it's used for |
| --- | --- | --- |
| USGS 3D Elevation Program (3DEP) | elevation.nationalmap.gov | Terrain elevation for slope, aspect, and winter sun hours |
| US Forest Service | apps.fs.usda.gov | Wildland-Urban Interface (WUI) status |
| US Forest Service data on the Federal GeoPlatform | imagery.geoplatform.gov | Wildfire hazard potential, burn probability, and tree canopy cover |
| FEMA National Flood Hazard Layer | hazards.fema.gov | Flood zone |
| US Census Bureau geocoder | geocoding.geo.census.gov | County lookup, and address-to-coordinates when needed |
| Esri World Geocoding Service | geocode.arcgis.com | Address-to-coordinates when the listing doesn't provide them, and a county lookup fallback |

Like any web request, these requests also reach those services with your IP
address and standard browser headers. Each service handles that information
under its own privacy policy. The extension sends no cookies, identifiers, or
account information of its own with these requests.

### Links you choose to open

The panel contains links — for example to a state or county parcel viewer,
ShadeMap, Google Maps, the FEMA flood map viewer, county tax records, or a web
search for a county parcel map. These links include the property's address or
coordinates. Nothing is sent to those sites unless you click a link, and once
you do, that site's own privacy policy applies. When you click a parcel-viewer
link, the extension also copies the property's address to your clipboard so
you can paste it into the viewer's search box.

## Free trial and purchase (ExtensionPay and Stripe)

LotScoop costs a one-time fee after a free trial. Payments and license checks
are handled by ExtensionPay (extensionpay.com), and card payments are
processed by Stripe (stripe.com). We never see or store your card details.

- **Before you start a trial or buy,** the extension does not contact
  ExtensionPay and you are anonymous.
- **When you click "Start free trial", "Buy LotScoop" or "Already paid?",**
  the extension asks ExtensionPay for a random license key for this browser
  and opens ExtensionPay's page. There you enter your **email address** (for
  the trial, or to log in to an earlier purchase), and at checkout Stripe
  collects your **payment details** and billing information on its own page.
- **License checks:** once a key exists, the extension asks ExtensionPay
  whether that key has an active trial or a purchase, when a Zillow page
  opens the panel and, while the panel is locked, when you return to the tab
  or once a minute. These requests carry the key, not the homes you look at.
- **What we can see:** ExtensionPay shows us, as the developer, the email
  address, trial start date, and payment status of people who start a trial
  or buy. Stripe shows us the purchase and the billing details needed for
  payouts, refunds, and taxes. We use these only to provide and support the
  license, handle refunds, and meet tax and legal obligations.

ExtensionPay and Stripe handle this information under their own policies:
ExtensionPay (see the "What about user privacy?" answer on
https://extensionpay.com) and the Stripe Privacy Policy
(https://stripe.com/privacy).

## What is stored, and where

LotScoop stores the following in `chrome.storage.local`, which lives **only on
your device** in your Chrome profile:

- tax figures read from listings you have opened, keyed by property address,
  so the tax row can be shown again when you see that home later; and
- the panel's position on the screen and whether it is collapsed.

ExtensionPay's script also stores, in `chrome.storage.sync`, the license key
for this browser, the date the extension was installed, and ExtensionPay's
last answer about your license (whether you have paid, when your trial
started, and the email you gave ExtensionPay, if any). LotScoop uses that
saved answer when ExtensionPay cannot be reached. If you have turned on
Chrome sync, Chrome syncs this storage area through your Google account, so
the license follows you to your other signed-in browsers.

Lookup results (elevation, hazard, and flood data) are kept only in memory
while Chrome is running, so re-selecting a home is instant; they are discarded
when the browser closes or the extension restarts.

Apart from the license key sent with license checks, none of this stored data
is sent to us or to anyone else. You can delete it at any time by removing the
extension at `chrome://extensions`; Chrome deletes an extension's stored data
when it is removed. Removing the extension does not delete your trial or
purchase record at ExtensionPay, so you can log in again later; ask us at the
address below if you want it deleted.

## What we do not do

- We do not operate servers that receive your data. We never see what homes
  you look at.
- No LotScoop account. The only sign-in is ExtensionPay's email link, used
  to start a trial or to restore a purchase on another browser.
- No analytics, telemetry, advertising, or tracking of any kind.
- We do not sell, rent, or share user data, and we do not use it for
  advertising, creditworthiness, or lending purposes.
- No remote code: all of the extension's code ships inside the package
  reviewed by the Chrome Web Store, including ExtensionPay's script. It only
  downloads data (not code) from the services listed above.

## Children

LotScoop is a general-audience tool for home buyers and is not directed at
children under 13. It does not knowingly collect information from anyone.

## Changes to this policy

If the extension's handling of data changes, this policy will be updated
before that version is published, and the effective date above will change. Material changes will
also be noted in the extension's Chrome Web Store listing.

## Contact

Questions about this policy or the extension: dan@escalantecloud.com
