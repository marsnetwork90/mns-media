# mns-media

Single source of truth for Mars Network Services and Mara marketing media. Buffer, the sites, email and Canva pull files from here by URL, so a URL in this repo is a published, stable address.

Raw URL pattern: `https://raw.githubusercontent.com/marsnetwork90/mns-media/main/<folder>/<file>`. The same paths serve through Cloudflare Pages at `https://media.themarsnetwork.com/<folder>/<file>` (and `https://mns-media.pages.dev/...`), with correct content types, long-lived caching and CORS from the `_headers` file. Prefer the media.themarsnetwork.com URL on the sites and in email; either works in Buffer and Canva.

Mara lobby, kiosk and industry images are AI-generated environments with real product screens composited on; nothing shows an invented interface.

## Rules

Filenames are lowercase with hyphens and no spaces, and they never change. Never overwrite a file with different content under the same name, because Buffer and the sites cache by URL; add a version suffix such as `-v2`, commit the new file, and update the table here. Only finished, publishable files live in this repo. Captures, plates, narration, masks and build scripts stay in the project folder.

Cloudflare Pages rejects any file over 25 MiB, so keep every file under that; re-encode video if needed.

Brand: Outfit typeface, navy `#1B2B4A`, red-orange `#E8452B`. See `_Shared/brand-assets.md` in the project for full rules.

## mara/video

Finished cuts only. Captures, plates, narration, masks and build scripts stay in the project folder.

| File | What it is | Where it is used | Raw URL |
|---|---|---|---|
| `mara-demo-60s.mp4` | Mara product demo, 62 s, 1920x1080 landscape | Facebook and LinkedIn feed posts, mara.themarsnetwork.com hero video, sales email | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/video/mara-demo-60s.mp4 |
| `mara-hook-vertical-25s.mp4` | Short hook cut, 25 s, 1080x1920 vertical | Instagram Reels, Facebook Reels and Stories | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/video/mara-hook-vertical-25s.mp4 |
| `mara-explainer-90s-v2.mp4` | Full explainer, 97 s, 1920x1080 landscape, 20.6 MiB (v2: re-encoded under the 25 MiB Cloudflare Pages limit; the 40 MiB v1 was never referenced and was removed) | Site explainer section, YouTube, sales follow-up email | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/video/mara-explainer-90s-v2.mp4 |

## mara/site

Assets for mara.themarsnetwork.com. Use the `-ui.jpg` versions on the site; the matching `.png` originals have a blank kiosk screen for any future re-composite. Never crop the AI disclosure out of a UI screenshot when the greeting text is visible.

| File | What it is | Where it is used | Raw URL |
|---|---|---|---|
| `hero-kiosk-lobby.jpg` | Kiosk on a lobby counter with the real greeting screen composited on, 1916x1080 | Hero poster frame behind the video, or the hero image until the video is approved | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/hero-kiosk-lobby.jpg |
| `hero-kiosk-visitor.jpg` | Same kiosk with a visitor standing at it, real greeting on screen, 1920x940 | Alternate hero, "Why a face" section | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/hero-kiosk-visitor.jpg |
| `hero-vertical-ui.jpg` | Vertical kiosk still with the real greeting screen, 1536x2720 | Mobile hero (9:16), story posts | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/hero-vertical-ui.jpg |
| `hero-vertical.png` | Vertical kiosk still, blank screen, 1536x2720 | Re-composite source only | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/hero-vertical.png |
| `lobby-wide.png` | Wide lobby from the entrance, kiosk on the far counter, 2720x1536 | Section background, "Built for businesses where the owner is never at the desk" | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/lobby-wide.png |
| `avatar-greeting-1080.png` | Mara mid-greeting, square crop from the kiosk, 1080x1080 | "Meet Mara" tile, about block, social profile | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/avatar-greeting-1080.png |
| `avatar-idle-1080.png` | Mara waiting, square crop from the kiosk, 1080x1080 | "Meet Mara" tile, about block, social profile | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/avatar-idle-1080.png |
| `avatar-popout.png` | Mara on a navy disc with red ring, transparent background, 577x665 | Anywhere she sits on navy | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/avatar-popout.png |
| `avatar-cutout.png` | Mara full cutout, transparent background, 1080x1080 | Anywhere she sits on navy | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/avatar-cutout.png |
| `ui-greeting.png` | Full kiosk greeting screen, 1920x1080 | "What Mara does" tile: greets | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/ui-greeting.png |
| `ui-checkin-all-set.png` | Full kiosk check-in confirmation screen, 1920x1080 | "What Mara does" tile: checks in | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/ui-checkin-all-set.png |
| `ui-booking-confirmed.png` | Full kiosk booking confirmation screen, 1920x1080 | "What Mara does" tile: books | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/ui-booking-confirmed.png |
| `ui-handoff.png` | Full kiosk human handoff screen, 1920x1080 | "What Mara does" tile: honest by design | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/ui-handoff.png |
| `sms-checkin.png` | Real staff text message for a check-in, raw, 1078x339 | "Pings your team" tile | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/sms-checkin.png |
| `sms-booking.png` | Real staff text message for a booking, raw, 1080x352 | "Pings your team" tile | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/sms-booking.png |
| `tile-sms-booking-1080.png` | Booking text message framed on navy, 1080x1080 | "Pings your team" tile, social | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/tile-sms-booking-1080.png |
| `calendar-event.png` | Real Zoho Calendar event, raw, 1080x1622 | "Books appointments" tile | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/calendar-event.png |
| `tile-calendar-1080.png` | Zoho Calendar event framed on navy, 1080x1080 | "Books appointments" tile, social | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/tile-calendar-1080.png |
| `dental-office-ui.jpg` | Dental front desk with the real greeting screen composited on, 2720x1536 | Industry section: Dental and chiropractic | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/dental-office-ui.jpg |
| `dental-office.png` | Dental front desk, blank screen, 2720x1536 | Re-composite source only | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/dental-office.png |
| `salon-front-desk-ui.jpg` | Salon front desk with the real greeting screen composited on, 2720x1536 | Industry section: Salons, spas and med-spas | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/salon-front-desk-ui.jpg |
| `salon-front-desk.png` | Salon front desk, blank screen, 2720x1536 | Re-composite source only | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/salon-front-desk.png |
| `contractor-office-ui.jpg` | Contractor office with the real greeting screen composited on, 2720x1536 | Industry section: Contractors and trades | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/contractor-office-ui.jpg |
| `contractor-office.png` | Contractor office, blank screen, 2720x1536 | Re-composite source only | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/contractor-office.png |
| `law-office-ui.jpg` | Law office reception with the real greeting screen composited on, 2720x1536 | Industry section: Law, accounting and real estate | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/law-office-ui.jpg |
| `law-office.png` | Law office reception, blank screen, 2720x1536 | Re-composite source only | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/law-office.png |
| `contractor-jobsite.png` | AI plate, contractor on a job site, no UI, 2720x1536 | Industry section, "the problem" section | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/contractor-jobsite.png |
| `salon-owner-phone.png` | AI plate, salon owner on the phone, no UI, 2720x1536 | Industry section, "the problem" section | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/salon-owner-phone.png |
| `empty-front-desk.png` | AI plate, empty front desk, no UI, 2720x1536 | "The problem" section | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/empty-front-desk.png |
| `mara-wordmark-accent-nolockup.svg` | Mara wordmark, navy letters with accent smile, no lockup line | Nav header on light backgrounds | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/mara-wordmark-accent-nolockup.svg |
| `mara-wordmark-accent-on-navy-nolockup.svg` | Mara wordmark, white letters with accent smile, no lockup line | Nav header on navy | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/mara-wordmark-accent-on-navy-nolockup.svg |
| `mara-wordmark-accent-on-navy.svg` | Mara wordmark on navy with the "by Mars Network Services" line | Footer, end cards | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/mara-wordmark-accent-on-navy.svg |
| `favicon.svg` | Smile-and-eyes on navy, 64 px | Favicon | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/site/favicon.svg |

## mara/wordmark

"mara" lowercase in Outfit Bold, outlined, with a single smile arc under the two a's. Colors: navy #1B2B4A, white, and the accent #E8452B on the smile only. Never color the letters red. PNGs are 2400 px wide with transparent backgrounds. Minimum size 25 mm for the badge file, 40 mm with the lockup line. Clear space at least the height of the m on all sides.

| File | What it is | Where it is used | Raw URL |
|---|---|---|---|
| `mara-badge-navy.svg` | Single-color navy badge mark, no lockup, no accent | Kiosk badge plate, 25 mm, engraving, embroidery | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-badge-navy.svg |
| `mara-badge-navy.png` | PNG of mara-badge-navy.svg | Same as the SVG where SVG is not accepted | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-badge-navy.png |
| `mara-badge-white.svg` | Single-color white badge mark, no lockup, no accent | Kiosk badge plate on a dark plate | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-badge-white.svg |
| `mara-badge-white.png` | PNG of mara-badge-white.svg | Same as the SVG where SVG is not accepted | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-badge-white.png |
| `mara-wordmark-navy.svg` | One-color navy wordmark with lockup line | Print, letterhead, anything one-color | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-wordmark-navy.svg |
| `mara-wordmark-navy.png` | PNG of mara-wordmark-navy.svg | Same as the SVG where SVG is not accepted | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-wordmark-navy.png |
| `mara-wordmark-navy-nolockup.svg` | One-color navy wordmark, no lockup line | One-color print where the MNS line is elsewhere | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-wordmark-navy-nolockup.svg |
| `mara-wordmark-navy-nolockup.png` | PNG of mara-wordmark-navy-nolockup.svg | Same as the SVG where SVG is not accepted | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-wordmark-navy-nolockup.png |
| `mara-wordmark-accent.svg` | Navy wordmark, accent smile, with lockup line | Site header, end cards, social on light backgrounds | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-wordmark-accent.svg |
| `mara-wordmark-accent.png` | PNG of mara-wordmark-accent.svg | Canva, Buffer, email on light backgrounds | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-wordmark-accent.png |
| `mara-wordmark-accent-nolockup.svg` | Navy wordmark, accent smile, no lockup line | Light backgrounds where the MNS line is elsewhere | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-wordmark-accent-nolockup.svg |
| `mara-wordmark-accent-nolockup.png` | PNG of mara-wordmark-accent-nolockup.svg | Canva, Buffer, email on light backgrounds | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-wordmark-accent-nolockup.png |
| `mara-wordmark-accent-on-navy.svg` | White wordmark, accent smile, with lockup line | Site header, end cards, social on navy | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-wordmark-accent-on-navy.svg |
| `mara-wordmark-accent-on-navy.png` | PNG of mara-wordmark-accent-on-navy.svg | Canva, Buffer, email on navy | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-wordmark-accent-on-navy.png |
| `mara-wordmark-accent-on-navy-nolockup.svg` | White wordmark, accent smile, no lockup line | Flyer and social headline, navy backgrounds | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-wordmark-accent-on-navy-nolockup.svg |
| `mara-wordmark-accent-on-navy-nolockup.png` | PNG of mara-wordmark-accent-on-navy-nolockup.svg | Canva, Buffer, email on navy | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-wordmark-accent-on-navy-nolockup.png |
| `mara-wordmark-white.svg` | One-color white wordmark with lockup line | Reversed, one color | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-wordmark-white.svg |
| `mara-wordmark-white.png` | PNG of mara-wordmark-white.svg | Same as the SVG where SVG is not accepted | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-wordmark-white.png |
| `mara-wordmark-white-nolockup.svg` | One-color white wordmark, no lockup line | Reversed, one color, MNS line elsewhere | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-wordmark-white-nolockup.svg |
| `mara-wordmark-white-nolockup.png` | PNG of mara-wordmark-white-nolockup.svg | Same as the SVG where SVG is not accepted | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/wordmark/mara-wordmark-white-nolockup.png |

## mara/flyers

Print and social graphics built with the Mara wordmark, MNS colors and Outfit. No prices on any flyer.

| File | What it is | Where it is used | Raw URL |
|---|---|---|---|
| `mara-flyer-letter.pdf` | US Letter print-ready handout, QR to mara.themarsnetwork.com | Leave-behind for builder offices, salons, dental and professional offices | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/flyers/mara-flyer-letter.pdf |
| `mara-social-square-1080.png` | Square social graphic, 1080x1080 | Instagram and Facebook feed posts, Meta static ads | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/flyers/mara-social-square-1080.png |
| `mara-avatar-popout.png` | Mara on a navy disc with red ring, transparent background, 577x665 | Flyer and social graphics | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/flyers/mara-avatar-popout.png |
| `mara-avatar-cutout.png` | Mara full cutout, transparent background, 1080x1080 | Anywhere she sits on navy | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mara/flyers/mara-avatar-cutout.png |

## mns/logo

Mars Network Services logo set. Flat navy and red-orange is primary. Icon versions only in circular crops; the lockup never goes in an avatar. Do not recolor, stretch or add effects. Gradient versions are a legacy option for Instagram only, never B2B.

| File | What it is | Where it is used | Raw URL |
|---|---|---|---|
| `mns-lockup-flat.svg` | Primary logo: navy M, red roof, company name | Website header, documents, proposals, cover images | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/logo/mns-lockup-flat.svg |
| `mns-lockup-flat.png` | PNG of the primary lockup, 2400x800 | Canva, Buffer, email signatures | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/logo/mns-lockup-flat.png |
| `mns-lockup-white.svg` | White lockup for dark backgrounds | Navy sections, dark cover images | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/logo/mns-lockup-white.svg |
| `mns-lockup-white.png` | PNG of the white lockup, 2400x800, transparent | Canva, Buffer, email on navy | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/logo/mns-lockup-white.png |
| `mns-lockup-gradient.svg` | Legacy gradient lockup | Instagram only, if at all | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/logo/mns-lockup-gradient.svg |
| `mns-lockup-gradient.png` | PNG of the gradient lockup, 2400x800 | Instagram only, if at all | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/logo/mns-lockup-gradient.png |
| `mns-icon-flat.svg` | Primary icon, flat navy and red-orange | Square and circular avatars, favicons, anywhere the name would be unreadable | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/logo/mns-icon-flat.svg |
| `mns-icon-flat-1024.png` | PNG of the flat icon, 1024x1024 | Social avatars, app icons | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/logo/mns-icon-flat-1024.png |
| `mns-icon-white.svg` | White icon for dark backgrounds | Kiosk badge plate, site footer on navy | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/logo/mns-icon-white.svg |
| `mns-icon-white-1024.png` | PNG of the white icon, 1024x1024, transparent | Canva, Buffer on navy | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/logo/mns-icon-white-1024.png |
| `mns-icon-navy.svg` | One-color navy icon | Invoices, stamps, embroidery | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/logo/mns-icon-navy.svg |
| `mns-icon-navy-1024.png` | PNG of the navy icon, 1024x1024, transparent | One-color contexts where SVG is not accepted | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/logo/mns-icon-navy-1024.png |
| `mns-icon-gradient.svg` | Legacy gradient icon | Instagram only, if at all | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/logo/mns-icon-gradient.svg |
| `mns-icon-gradient-1024.png` | PNG of the gradient icon, 1024x1024 | Instagram only, if at all | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/logo/mns-icon-gradient-1024.png |
| `mns-facebook-cover.png` | Facebook page cover, 1640x624 | Facebook page header | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/logo/mns-facebook-cover.png |
| `mns-linkedin-banner.png` | LinkedIn company page banner, 4200x700 | LinkedIn company page header | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/logo/mns-linkedin-banner.png |

## mns/fonts

Outfit is the brand typeface. Serve these from media.themarsnetwork.com with `@font-face` or upload them to the Canva Brand Kit.

| File | What it is | Where it is used | Raw URL |
|---|---|---|---|
| `Outfit-Bold.ttf` | Outfit Bold, TrueType | Headlines, wordmarks, site headings, Canva Brand Kit | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/fonts/Outfit-Bold.ttf |
| `Outfit-Regular.ttf` | Outfit Regular, TrueType | Body copy, site text, Canva Brand Kit | https://raw.githubusercontent.com/marsnetwork90/mns-media/main/mns/fonts/Outfit-Regular.ttf |
