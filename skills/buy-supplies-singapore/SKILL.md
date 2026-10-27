---
name: buy-supplies-singapore
description: Get a firm SGD price and delivery date for office, IT and electronics supplies, ink and toner, or event print in Singapore, then help the buyer place the order. Use when someone in Singapore needs cables, adapters, storage, peripherals, monitors, UPS, networking gear, printer supplies, name cards, lanyards or banners delivered.
---

# Buying supplies in Singapore

Use the Singapore Buying Desk tools. The desk is operated by Connective Labs Pte. Ltd. (UEN 202543350R), which is the merchant of record and invoices the buyer's company.

## 1. Pin down the item before quoting
Ask only for what changes the price, then quote:
- Cables and adapters: connector on each end, length, version if it matters (HDMI 2.1, Cat6).
- Storage: type (USB flash, microSD, SSD, HDD), capacity, interface (USB-C, SATA, NVMe).
- Ink and toner: printer brand and cartridge code (e.g. HP 206A), colour, quantity.
- Peripherals, monitors, UPS, networking: brand and model if known, otherwise the key spec (size, VA rating, ports).
- Print and merch: item, quantity, size, artwork ready or not.
Always ask for quantity and the date it is needed by.

## 2. Quote
- One office, IT, ink or toner item: call `quote_office_supplies` with the buyer's wording, `quantity` and `needed_by`.
- Several items at once: call `quote_list` once with all lines.
- Name cards, lanyards, banners, totes: call `quote_event_print`.
- No match, or a custom spec: call `request_quote` with every known detail; a firm quote comes back by email, usually the same business day.

## 3. Present honestly
- Prices are SGD, include 9% GST and Singapore delivery, and are refreshed daily from trade quotes. Stock and price are confirmed at order; never call them live.
- If a result is a similar item rather than the exact model, say so.
- Show the ready-by date next to the price.

## 4. Order
Only place an order after the buyer approves the exact item, quantity, price and delivery address. Use `request_quote` with the approved details and the buyer's email. No payment is taken in chat: the buyer receives a firm quote and pays by PayNow or a payment link in the company's name. Full refund if the confirmed date is missed.

## Do not
- Do not quote for delivery outside Singapore.
- Do not ask for card numbers.
- Do not charge or place an order without the buyer's explicit approval of the firm quote.
