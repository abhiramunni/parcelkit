# ParcelKit — Track Every Delivery in One Place

Every parcel. One place. No more “where is my order?” ParcelKit keeps every order you are waiting for — its courier, tracking ID, expected day and return window — right here on your device. Nothing leaves it.

**Live:** https://abhiramunni.github.io/parcelkit/

## What it does

- **Next delivery card** — the parcel landing soonest, with a days-to-go ring, courier and tracking ID. Overdue parcels get the attention banner instead of the hero spot.
- **Arriving wall** — everything still on its way, soonest first. Each card shows the expected date, price, a 5-stage pipeline (Ordered → Packed → Shipped → Out for delivery → Delivered) and a status pill (Arriving today / tomorrow / in N days / Needs attention).
- **Move it along** — tap “Move one step” as the courier updates, or “Mark delivered” when it lands. The return clock starts on the delivery day.
- **Delivered archive** — every delivered parcel with its return window counted down in days, so a 7-day return never slips past.
- **Needs attention** — any parcel past its expected date is flagged in the stats, the banner and its own filter.
- **Track on the courier’s site** — one tap opens Amazon order history, Flipkart orders, or the courier’s tracking page (Delhivery, Blue Dart, DTDC, Ecom Express, XpressBees, India Post). The tracking ID copies with one tap.
- **Add a parcel in 30 seconds** — item, courier, tracking ID, expected date, price and return window. Notes too (“Gift for Appa — don’t open early”).
- **Search + filters** — All, In transit, Out for delivery, Needs attention, Delivered, plus free-text search across item, courier and tracking ID.
- **Your numbers** — parcels in transit, arriving this week, delivered this month, parcels needing attention, and what you spent on parcels this month.
- **6 plain-language guides** — finding a tracking ID, a stuck parcel, return windows, COD safety, damaged boxes, and making sure the delivery finds you.
- **Copy my summary** — a plain-text list of what’s coming and what’s delivered, ready to paste anywhere.
- **Remove samples / erase everything** — the starter parcels clear out in one tap; erase is two-tap so it never happens by accident.

## Seeded parcels

Seven realistic starter parcels (use “Remove samples” to start from your own): boAt Airdopes 141 arriving tomorrow, a white linen shirt, a phone case, college textbooks by India Post, a Bluetooth speaker 3 days overdue, plus two delivered parcels with live return countdowns. Stats on load: 5 in transit, 3 arriving this week, 2 delivered this month, 1 needs attention, ₹11,090 spent this month.

## Design

Warm editorial palette (ivory paper, espresso ink, bronze/amber/gold/terracotta), Fraunces + Inter, full-screen cinematic intro with tap-to-skip (quick on return visits), slow Ken Burns drift on the two AI-generated parcel photos, a vertical timeline wall with a dashed route line, and a 3-step onboarding coach.

## Tech

Single self-contained `index.html` — no backend, no signup, no build step. All data lives in `localStorage` on the device. Works offline once loaded. Courier links open the courier’s own site; ParcelKit never checks a tracking number itself.

## Privacy

No account, no server, no sync, no analytics. Your tracking IDs and prices stay in your browser’s local storage and nowhere else.
