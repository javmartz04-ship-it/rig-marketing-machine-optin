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
