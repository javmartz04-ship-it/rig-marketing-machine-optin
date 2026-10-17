# RIG: The Marketing Machine, webinar registration (2026-10-09)

**Brief (Javier):** a new opt-in for Johnny Brock's Marketing Machine webinar, Saturday 11AM EST.
Use the Tuesday opt-in (therealinsurancegroup.com/optin-186491) as inspiration but make it better.
No video: make it feel like a webinar, with a picture of one and some of the slides. Keep "Here's
exactly what I'm covering" and Johnny. Use the deck's colors.

**Preview:** https://javmartz04-ship-it.github.io/rig-marketing-machine-optin/ (repo of the same name; push to update).

**Direction:** the deck's whiteboard register, lifted exactly from `~/Desktop/Jarvis/rig-marketing-machine/src/v4.css`:
paper #F6F5F1, ink #0B1220, yellow highlighter on the key words, ink-bordered cards with hard
offset shadows, pastel icon tiles (same SVGs as slide 5), Inter Tight + Caveat + JetBrains Mono
(the deck's own font files). Logo is the white logo.webp with `filter:brightness(0)`, as the deck does it.

**Structure:** full-width 2-line H1 (emphasis = "predictable machine." in highlighter) → split:
sub + countdown + CTA left, a fake webinar window right (screen-share rotating through 4 real
slides, Johnny's cutout as the cam tile, LIVE chip, Q&A button, title slide tilted behind) →
3 stats (2020 / $137K / 4,000+, from deck slide 3) → problem 01–03 → reframe ("You don't have a
lead problem. You have a machine problem.") → the five parts as tiles → agenda 01–06, each row
paired with the real slide → host (on-stage photo) → 3 real testimonials → for / not for → dark
final CTA with countdown and a slide stack. CTA "Reserve My Free Seat" everywhere.

**Proof rule applied:** the old Tuesday page had 8 testimonials, most with names not found in
any deck (and Thomas Key's quote attributed to "Carla Whitfield"). Only the three in the deck
(Jill Coates, Mindy Baron, Thomas Key) were used.

**Form:** same modal and fields as the Tuesday page (name, email, phone → GHL inbound webhook),
but `WEBHOOK` and `THANKS` are empty at the top of the script, so the preview sends nothing and
shows the inline success state. The Tuesday webhook was NOT reused (it would enroll people into
the Tuesday sequence). Needs the Saturday webhook + thank-you URL from Javier.

**Countdown:** next Saturday 11:00 America/New_York, DST-aware, shows "We're live right now" for 90 min.

**Webhook wired 2026-10-09:** 6c582ec4… (Saturday). **Open:** thank-you page, which Saturday (countdown just targets the next one), whether
the 3,459 leads at $1.64 veteran-campaign line is OK on a public page.

**2026-10-11:** first Saturday run went well ("crushed"); it's now an every-Saturday webinar (countdown already rolls weekly). Fixed the cam tile: a generic `.win .screen img` rule (height:100%, object-fit:cover) was cropping Johnny's forehead; the cam img now overrides it with height:auto.

**2026-10-11:** real RIG logo (gold/silver, from Javier) cut out of its black background to a transparent webp (assets/rig-logo.webp). It's in the webinar window bar, the final CTA box and the footer. The old black checkmark logo.webp is gone. The slide screenshots still show the old logo on slide 01.

**2026-10-11:** two video testimonials added above the text quotes (from Javier's Desktop): Barry, agency owner with 7 employees, 20 → 50 deals a week (no last name given); and the ASL agent, labelled Justin Gray from the ASL client memory, not stated in the clip. 720x1280 H.264 + whisper VTT captions in assets/video; poster frames picked so the face is clear; the play button sits at the bottom so it doesn't cover faces.

**2026-10-11:** testimonial headlines per Javier: Barry = "Scaled to 50 / deals a week, up from 20"; Justin = "$12 / booked appointments in the ASL market" (Javier's framing; the clip itself says leads at ~12 bucks). Mobile pass at 360/390/430: no horizontal overflow; pill + webinar bar no longer wrap; the five parts become compact icon rows under 720px.

**2026-10-11 thank-you page (thanks.html):** concept = a seat ticket (ADMIT ONE, live date from the weekly Saturday logic, red SEAT RESERVED stamp that lands on load, countdown on a cream stub, decorative barcode). Google Calendar link + .ics download with a 30-min alarm, 3 next steps (text/email, bring your numbers, show up live), auto-scrolling strip of real slides, dark sign-off with Johnny cutout on a yellow disc. Opt-in still shows its inline success state until `THANKS` gets the GHL thank-you URL.

**2026-10-11 thank-you v2:** calendar buttons removed (Javier: GHL sends the reminders, don't promise calendar adds). Hero now has a 3-step "what happens next" card (confirmation now, updates before Saturday, link the day of). Step 01 says updates before the presentation + link the day of. Strip trimmed to 3 slides on repeat.

**2026-10-11:** THANKS = https://therealinsurancegroup.com/confirmed (live GHL page, carries thanks.html). Redirect tested with the webhook stubbed (no test contact sent). Javier: no temporary links in the funnel. Only the asset files (fonts, images, videos) still load from GitHub Pages, so the rig-marketing-machine-optin repo must stay up.
