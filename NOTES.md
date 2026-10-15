# Amanda Camp & Co: open items

Private working list. Netlify is set to return a 404 for this file (see `netlify.toml`), so it is not visible on the live site.

## Proof still needed (the site's claims are strongest with real numbers)
- [ ] **A real AI-cost figure.** One concrete number beats any claim: a monthly AI bill you cut, tokens or dollars saved by switching models or trimming prompts, or the cost of running the Command Center per month. Add it to the "Why most AI spending doesn't pay off" section and the stats band.
- [ ] **An "unused tool" story.** A real case of a tool or subscription that was dropped or never adopted, and what replaced it.
- [ ] **A prompt/skills example.** Before/after of a team prompt turned into a reusable Claude skill (with the time saved).
- [ ] **First client result + testimonial.** Replaces the in-house results note under the stats band.

## Before the site goes public
- [x] Employer sign-off on using the Command Center video, cash forecast, card controls and the stats. (Yes, received 2026-10-15. Keep the written reply somewhere safe.)
- [ ] Nate blurred in the demo video. A blurred version was made (tracks his name frame by frame) and re-scanned: it caught nearly everything but one moment around 14s (the Awards line, "currently with Nate") still leaks. Not shipped. The live video still shows Nate. Finish the pass, or swap in a still image, before going public.
- [ ] Decide on the Vederra logo in the video (still visible).
- [ ] Remove `noindex` from `index.html` when ready for Google.
- [ ] Netlify: DNS verified, certificate issued, `amandacampco.com` primary.
- [ ] Set up hello@amandacampco.com and swap it for the Gmail address.
- [x] Contact form added (Netlify Forms). **Still to do in Netlify:** after the first deploy, open Forms and confirm "contact" appears, then Forms → Form notifications → add an email notification to amandacampco@gmail.com. Send yourself a test message.
- [ ] **Booking link.** Create the page (Google Calendar: Create → Appointment schedule, or Cal.com), copy its public URL, paste it into `<meta name="booking-url" content="">` in `index.html` (or send it to Claude). A "Book a time on my calendar" button then appears beside the form. Suggested page: title "Free intro call: Amanda Camp & Co", 30 minutes, 15 minute buffer after, 24 hours minimum notice, ask one question: "What's eating your week, or what are you paying for that isn't working?"
- [ ] **Analytics (free).** Umami Cloud Hobby plan (no cookies; free tier lists 1 site, 100K events a month, 6 months of history; confirm their terms allow business use). Sign up, add amandacampco.com, copy the Website ID, paste it into `<meta name="analytics-id" content="">` in `index.html` (or send it to Claude). Events already wired: section views, hero/nav/form/email/booking clicks, form sent, video unmuted. Visitors with Do Not Track on are not counted.
- [ ] Add a "starts at $X" line once pricing is set.


## Proof log (collect this for every project, including paid pilots and in-house work)
One row per project. Real numbers only; mark estimates as estimates. Get written permission before publishing.

| Project | Date | Problem in one line | Before (hours/week, $/month, errors) | After | Who uses it weekly | AI cost per month (API, subscriptions) | Quote (with permission) | OK to publish? |
|---|---|---|---|---|---|---|---|---|
| Marketing Command Center | | | LinkedIn under 100 impressions/month | 13,431 impressions in May 2026 | | | | Employer said yes (2026-10-15) |
| Card Controls | | | | 96% of 338 charges cleared automatically | | | | |
| Onboarding with Claude | | | | 100+ hires, 53 offer letters in one week | | | | |
| This website | | Needed a business site | | Brief to live site built with Claude | n/a | | | n/a |

**Where to get the cost numbers:** the Anthropic Console usage page (spend by model and day), Claude Code's cost view for sessions, and subscription invoices. Record the month before and the month after any change that was meant to cut cost (cheaper model, shorter prompts, caching).

## Website measurement plan
Track weekly in one place (a simple sheet): visits, where they came from (LinkedIn, referral, direct), contact-form messages, calls booked, replies from outreach, calls that became paid work.
Targets for the first two weeks after launch: send to 10 target owners and 3 fractional CFOs; success is 2 of 13 booking or replying with a real question.
Add after launch: analytics on the site (Netlify Analytics needs no code), and a booking link.
