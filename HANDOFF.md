# Home Again Cleaning Services — handoff at ~60%

**Live:** https://10elizabethbell.github.io/homeAgainCleaning/ · **Repo:** https://github.com/10elizabethbell/homeAgainCleaning · **Built:** 2026-10-20 from Muse brief 2026-10-20 (Toms River Connections group post, thin brief) · **Call Sheet:** site set

## What's built
- One page, phone first, calm band style: paper header → navy hero → paper "peace of mind" → deep-navy services → paper estimate form → navy close → deep footer.
- Hero is the **plain textured navy band**: the business has no photos and no logo anywhere (text-only post), so nothing could go behind it. H1 "Your Ocean County home, clean again." bounces in letter by letter; promise line is their own caption.
- Palette (builder's choice, no brand colours exist): paper #f4f6fb, harbour navy #1f4a7a, deep #10233f, sparkle gold #f5c64f (fills; #7f5a00 as text on light). Gold taken from the ✨ in their post title.
- Services: their 7 verbatim services as short rows; tapping one jumps to the form with that service pre-picked.
- **Contact is Facebook Messenger only** (no phone/email exist): header "Message us", form, closing button and the floating circle all go to `https://m.me/100006322602656` (the poster's profile id, decoded from the post's `fb://` link). The form writes the message, copies it, and shows it with an "Open Messenger" button, because Messenger links can't carry a pre-filled message.
- **Phone switch is built in:** set `CONFIG.PHONE` and `CONFIG.PHONE_LABEL` at the top of the script and the header becomes a tap-to-call number, the form sends a pre-filled text, and the close button and circle become "Text us".
- Favicon, touch icon and og.png use the site's own lettering (an "H" with a gold sparkle), since there's no logo.

## Assumptions I made
- **"We" voice**: their captions say "Let us…", "Message us…".
- **Owner not named**: the brief says Lynne Grau's relationship to the business is unconfirmed.
- **Messenger goes to the poster's personal profile** (id 100006322602656). That's where the ad sends people, but it's a personal account; the footer "Facebook" link also points there. Confirm with the owner before handing over.
- "Cleaning tailored to your home" and "Dependable and detail-oriented" are shortened from their "Personalized cleaning tailored to your needs" / "Dependable, detail-oriented service".
- The care paragraph ("You're trusting us with the place you come home to…") is my copy in their tone, not theirs.
- Audience: not marked 40+, so the calm motion stays. Ocean County skews older (big retirement communities); if Ellie wants, switch to `older-audience.md` (no bounce-in, no fade-up, bigger type).

## Placeholders and gaps
- No phone, no email: the footer has no email (rule: never invent one). Phone switch is ready in `CONFIG`.
- No photos, before/afters, reviews, prices, hours, years in business: page says nothing about them.
- No mid-page "see more of our work on Facebook" link, because there's no work to see and no business page; Facebook is in the footer only.
- `m.me/<numeric id>` for a personal profile is **not verified** to open a chat (couldn't test logged in). If it fails, set `CONFIG.MESSENGER` to `m.me/<username>` or `https://www.facebook.com/messages/t/100006322602656`. Also worth trying `?text=<message>` on the link; if Messenger pre-fills it, the copy/paste step can go.
- Messages from non-friends land in Messenger's **Message Requests** folder; tell the owner to check it.
- No phone number exists, so the header's top-right slot holds "Message us" instead of a number (the house rule wants a number there once one exists).

## Questions for the owner
- Best phone number, and does it take texts? Email for the footer?
- Is Lynne the owner? OK to name her ("I'm Lynne…") and add a photo?
- Would they make a Facebook business page (cleaner Messenger link, a place for photos and reviews)?
- Any before/after photos of their cleans, and client reviews they can share?
- Which towns do they cover most (Toms River, Brick, Lakewood…)? Hours? Prices or a starting rate?
- Insured/bonded? Supplies included? Pet-friendly products?

## Ideas not built (yours to pick)
- **Impeccable findings kept against, because they're the house calm style:** eyebrow pills (craft floor bans eyebrows), the diagonal band texture (detector "repeating stripes", suppressed for index.html in `.impeccable/config.json`), the same fade-up on each section, 24px cards and pill controls.
- Wait for Cal Sans to load (about 300ms cap) before splitting the H1, so the bounce-in doesn't reflow when the font arrives.
- A small sparkle twinkle beside "Your message is copied".
- **Runner-up worlds (opt-in signature motion):** (1) a sunlit window the visitor wipes clean with a finger, streaks to sparkle (best fit: "clean again"); (2) soap bubbles drifting up the hero that pop on tap; (3) a fresh-linen fold line that ripples; (4) a squeegee sweep across the hero; (5) dust motes in a sunbeam that clear when touched.
- Seasonal hook from the brief: a short "Holiday cleaning" or "Airbnb turnover season" line once the owner confirms availability.
- A "Who we look after" strip (homes / vacation rentals / offices) once there are photos for each.
- Desktop hero right side is empty; a client photo would fill it once one exists.

## Not verified
- Real-device Messenger handoff from Facebook's in-app browser (iOS and Android), including clipboard copy there.
- Real-device touch and frame rate on older phones.
