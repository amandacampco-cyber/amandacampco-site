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
- [x] Booking link: decided against it for now. The form collects "best times to talk" and replies set up the first calls by hand. Add a scheduling page later once your availability is settled.
- [x] **Analytics (free):** Umami Cloud, website ID is in the `analytics-id` meta tag in `index.html`. Events wired: section views, hero/nav/form/email clicks, form sent, video unmuted. Visitors with Do Not Track on are not counted. Confirm the first visit shows in the Umami dashboard after the site is live. Check their terms allow business use on the free plan.
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
Analytics is on (Umami). No booking link yet; first calls are set up by reply.


## Brand system: "The Sunday Edition" direction (set 2026-10-15)
Cozy, modern, newspaper-inspired. Editorial, warm, trustworthy, practical. Not a 1920s newspaper, and not the glowing blue/purple look most AI consultancies use.
- **Colors:** paper cream `#F6EFE4`, ink `#1F1E1A`, olive `#6B7058`, taupe `#B7A899`, rust `#B75E46` (buttons use the slightly darker `#A4503A` for contrast), stone `#DAD4C8`.
- **Type:** Newsreader (headlines, body, italic accents) and Figtree (small uppercase labels, buttons, nav).
- **Devices:** masthead with dateline and double rule, numbered section labels ("01 /"), column rules instead of boxed cards, "Fig. 1" captions, "Editor's note", boxed "Case study" tags, circular AC seal.
- **Photography (still needed):** warm, muted, natural light, breathing room, a personal feel (desk, books, coffee, plants, Colorado light). Avoid AI-generated stock images. Real photos of your workspace beat anything generated, and the headshot needs a larger, uncropped version.
- **Open positioning question:** stay focused on "AI that gets used" (current), or broaden to "better systems" with websites, dashboards and operations as services. Current choice: AI-enabled business improvement is the central idea; add dedicated service pages later.

## Client hosting policy (set 2026-10-15)
**Rule: never run live client sites on your free personal Netlify account.** Credits are shared per account. If the pool runs out, every site on it is paused at once, clients included.

**Default: the client owns their hosting.**
1. The client creates their own Netlify account (free plan fits most small sites). Check Netlify's terms on commercial use first.
2. The site's code lives in a GitHub repo that you transfer to them or keep under their organization, with you added as a collaborator for maintenance.
3. The client's domain DNS points at their Netlify site (A record `75.2.60.5` for the bare domain, CNAME for `www`; use whatever values Netlify shows).
4. You hand over admin access and a one-page "how to edit and publish" guide.

**Optional: managed hosting (a "site care plan").** You host on a paid plan and bill a monthly fee that covers it, plus updates, backups and a monthly check. Netlify Personal is $9 a month for 1,000 credits and Pro is $20 a month for 3,000 credits with unlimited members; credit packs are $5 per 500 on Personal and $10 per 1,500 on Pro. Move to Pro once you manage three or more sites. **Set the care-plan price so it clearly covers the plan cost.** (Price: to be decided.)

**Credit math (Netlify credit-based plans):** production deploy 15 credits, bandwidth 20 per GB, web requests 2 per 10,000, form submissions free, deploy previews and branch deploys 0. So 300 credits is about 20 deploys in total, 1,000 is about 66, 3,000 is about 200.

**Habits that save credits on every site**
- Batch changes. One release is one production deploy.
- Test on branch deploys or deploy previews (0 credits), then publish once.
- Host large videos on YouTube (unlisted) or Vimeo and embed them.
- Add `[skip ci]` to commits that change only notes, so they do not trigger a deploy.

**Proposal wording (copy and adjust)**
> *Hosting and domain.* Your website is hosted on a Netlify account that you own. For most small sites this costs $0 a month on Netlify's free plan; busier sites may need a paid plan. Your domain renews with your registrar each year. I set everything up, hand you full access and a short guide, and you stay in control.
>
> *Optional site care plan: $___ per month.* I host your site, apply updates, keep backups and check performance monthly, so you never have to manage it.

**To decide:** care-plan price; which Netlify plan you will manage client sites on; whether the first client pilot is free or discounted in exchange for a quote and results.

## Security baseline (set 2026-10-15): for this site and every client site
A static site (plain HTML on Netlify) has no database, no logins on the page and no plugins, so classic malware is rare. The real risks are **account takeover, form spam, fake email from your domain, DNS/domain hijack, and third-party scripts.**

**Already done on this site (netlify.toml)**
- Security headers: Content-Security-Policy (only your own files, Google Fonts and Umami can load), no framing by other sites, no content-type sniffing, strict referrer policy, camera/microphone/location blocked, HTTPS enforced by Netlify.
- Contact form: hidden honeypot field. Netlify Forms also filters spam on its side (check the Forms tab for a "Spam" list; confirm current options in Netlify).
- Private notes are hidden from the public site; no secrets are stored in the repo.
- Cookieless analytics, off for visitors with Do Not Track.

**Your checklist (accounts are the biggest risk)**
- [ ] Turn on two-step verification, ideally passkeys, for: Netlify, GitHub, Spaceship (domain registrar), Google, Umami. Use a password manager, unique passwords.
- [ ] Spaceship: confirm the domain's transfer lock is on and auto-renew is on (auto-renew already shows On). Consider enabling DNSSEC if offered for your DNS setup.
- [ ] Netlify: check Team members and remove anyone who should not have access; never share one login. Keep deploy tokens and API keys out of the repo.
- [ ] GitHub: keep repos private; turn on secret scanning if offered; require 2FA for anyone you add.
- [ ] Form spam: if junk appears, turn on reCAPTCHA in Netlify's form settings (adds a Google script, so update the CSP in netlify.toml), or add a short time-delay check.
- [ ] Email from your domain (when hello@amandacampco.com exists): set up SPF and DKIM as your email provider instructs, then add a DMARC record in Spaceship DNS: TXT, host `_dmarc`, value `v=DMARC1; p=none; rua=mailto:amandacampco@gmail.com` to start, tighten to `p=quarantine` after a few weeks. Until you send email from the domain, a stricter alternative is TXT `@` = `v=spf1 -all` and `_dmarc` = `v=DMARC1; p=reject;`, which stops others faking your address.
- [ ] Monitoring: free uptime check (for example UptimeRobot) on both domains, and Google Search Console (it warns about hacked content). Look at Netlify's Deploys list monthly for deploys you did not make.
- [ ] Backups: GitHub holds the full site history and Netlify keeps old deploys. Note where each client's repo and domain login live.

**For client sites (add to every project)**
1. Client owns the Netlify, GitHub and domain accounts, each with two-step verification on. You get named collaborator access, not their password.
2. Start from this site's `netlify.toml` headers. Edit the Content-Security-Policy to match only the scripts that site really uses; test after changing it.
3. Forms: honeypot on every form, Netlify's spam filtering, add reCAPTCHA if spam shows up.
4. Prefer plain static sites for brochure and lead-generation pages. If a client needs WordPress or a similar CMS, that is where malware lives: use a managed host, automatic updates, few plugins, a security plugin, limited admin users, and offsite backups, and price it into a care plan.
5. Keep third-party scripts to a minimum and list each one in the handoff doc.
6. Email authentication (SPF, DKIM, DMARC) for the client's domain, and a monthly check of uptime, forms and deploys inside any care plan.
7. Put "how we handle security" in the proposal and handoff guide so clients see it as part of the value.

**What no headline setting can fix:** a stolen password or a phished login. That is why two-step verification comes first.
