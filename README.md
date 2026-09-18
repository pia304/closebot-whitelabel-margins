# closebot white label: how agencies rebrand AI setters, set their own pricing, and rebill clients

The search "closebot white label" almost always comes from the same place: an agency owner who already knows CloseBot books appointments, and now wants to know whether they can hand it to clients with their own logo on it — and whether the money math works.

Short answer: yes, but two things get mixed up constantly. First, white labeling is locked to the Agency plan, not something you switch on in the free tier. Second, what gets your logo is the client portal, not the entire CloseBot app. Your clients log into a branded dashboard; you log into the actual builder. That split is deliberate, and once you see why, the pricing starts to make sense.

## What actually gets white-labeled in CloseBot

CloseBot's homepage puts it plainly: white-label with your name, your domain, your branding, and run appointment-setting agents for every client from one dashboard. In practice, the branded surface is the client portal plus the client-facing experience around it.

Here is the honest breakdown of what carries your brand and what doesn't:

- **Client portal** — your domain, colors, and logo. Clients see their agent performance and their own usage costs, not the same KPIs you see.
- **Client view of agents** — clients fill in predefined variables (business info, services, amenities) and upload knowledge base documents. They get the personalization controls, not the logic.
- **Agent building** — yours only. In V2, only your agency account can create and edit agents. That was a deliberate change from V1, where sub-accounts could build their own bots and, per CloseBot's own writeup, would "go in and break things."
- **The app itself** — still app.closebot.com. You and your team work inside CloseBot; your clients never see the builder.

That last point matters if you were hoping to resell a fully unbranded platform with your own login screen. You aren't getting that. You're getting a branded client-facing layer on top of a tool you operate.

For most agencies that's the better trade anyway. The value you're charging for is your build and your oversight, not a blank login page.

## The Agency plan is the gate — and the $397 question

CloseBot doesn't hide this. The [plans page](https://app.closebot.com/a?fpr=li87) separates the two tracks explicitly: business plans come with message costs included in the base price, agency plans come with client re-billing and white labeling.

The part people miss is on the business side. Even during the 7-day agency trial, the business plan simply doesn't show you the re-billing and white-label screens. If your plan is to sell AI setting under your own brand, the business track is a dead end, no matter how many agents you're running.

Agency pricing as currently listed:

- **$397/month** on monthly billing
- **$331/month equivalent** on annual billing, charged as $3,970/year

That's roughly $792 a year difference for switching to annual, and annual plans also unlock the larger 50+ template library instead of the 15+ on monthly. If you're confident you're keeping this in your stack, the annual switch is close to free money.

Compared against the agency subscription you're probably already paying for elsewhere, the number isn't outrageous. The question is whether the rebilling margin covers it. For most agencies running even a handful of clients, it does — more on that below.

## What your clients see (and what stays yours)

This is the design decision that makes white labeling work, and it's worth understanding before you sell it.

When a client logs into their branded portal, they see:

- Their agent's responses, conversations, and booked appointments
- Their own usage and costs
- The variable fields you defined for their industry
- The knowledge library where they can upload their own documents

They don't see your job flow logic, your personas, or how the sausage is made. One agent can serve unlimited accounts within the same niche, with each client filling in their own details through variables you set up in advance. If you build one gym agent with an `amenities` variable, every gym client personalizes their own version in a few clicks — and you didn't rebuild anything.

The knowledge library piece has a quiet upside. Clients upload their own files, storage gets billed to you at the agency rate, and you can mark it up. The more diligent your clients are about uploading context, the better their agent performs and the more that line item earns.

## The rebill math: turning usage costs into agency margin

Rebilling is the reason the Agency plan exists, and it works through Stripe. You connect a Stripe account, enable rebilling in account settings, set your markup rates, and then decide per client whether it's on.

Three things are rebillable:

1. **Message responses.** The plans page currently lists the agency rate at $0.012 per message, and you set whatever markup you want on top. Most agencies mark up messages rather than AI provider tokens, since token costs move around and are hard to explain to a client.
2. **User seats.** CloseBot charges $5 per additional seat per month and bills it incrementally by the hour, so mid-month additions don't create awkward rounding. Clients who want portal access count as seats. You can mark these up too.
3. **Knowledge library storage.** Billed to you at $0.006 per MB per day, and entirely markable-up. As the docs put it, the more your clients upload, the more you get paid.

Your clients top up their own wallet, which pays you through your Stripe account. You top up yours, which pays CloseBot. The gap is yours. You can also adjust the upcharge per client, per item, which matters when one client is a squeaky clean 300-message-a-month account and another is a high-volume monster.

How much can that be worth? CloseBot's own pricing page says polled agencies bill an average of $500 per client per month, and it advertises agencies earning up to 5x more per client than with native CRM tools. Those are vendor numbers, not audited ones. A more concrete data point from CloseBot's own case studies: Nick Tan builds CloseBot setups for $5,000 up front and $500/month ongoing, and built his agency model around it.

Do the rough version yourself. Ten clients at $500/month is $5,000 in monthly billing against a $397 platform fee and usage you've already marked up. Even at three clients the subscription is covered with room left. The catch is that none of this works if you can't build an agent that books — the rebilling dashboard just scales whatever you actually deliver.

## All CloseBot plans, side by side

Everything currently shown on the official pricing page, including the plan most people browsing for "white label" will never use:

| Plan | Best for | Key configuration | Price | Billing | Purchase link |
| --- | --- | --- | --- | --- | --- |
| **Free** | Testing, or under 100 replies a month | 100 AI replies/month, 1 agent, 1 user seat, 1 MB knowledge storage, unlimited account connections, no white labeling | $0 | Always free, no credit card | [ 免费注册 CloseBot 账号](https://app.closebot.com/a?fpr=li87) |
| **Core (Business track)** | Businesses automating their own pipeline | Message costs included in base price, 15+ templates, human support, extra users at $5/seat, add-on storage, add-on agents; no rebilling or white label | From $64/month ($53/month equivalent billed as $640/year) | Monthly or annual | [ 查看 Business 套餐](https://app.closebot.com/a?fpr=li87) |
| **Core (Agency track)** | Agencies building and rebilling agents for clients | Unlimited agents, re-bill all costs, white-label client portal, messages at $0.012 rebillable, seats at $5, storage at $0.006/MB/day, 50+ templates on annual | $397/month ($331/month equivalent billed as $3,970/year) | Monthly or annual | [ 开通 Agency 套餐并开始 white label](https://app.closebot.com/a?fpr=li87) |
| **Growth** | Teams needing SLAs, compliance, or high volume | HIPAA compliance, quarterly audits, 99.99% priority uptime, priority support, 50+ templates, custom scaling | Custom quote | Contact sales | [ 咨询 Growth 定制方案](https://app.closebot.com/a?fpr=li87) |

A few notes that the table can't hold. Business pricing scales with the monthly reply volume you select on the plans page slider, which runs from 100 replies up to 100K+; business plans include message costs in the base price unless you exceed your ceiling, after which overage draws from your wallet at a higher rate. Agency accounts are billed per message instead, because usage has to pass through to clients for rebilling to work.

If you've seen older numbers floating around — $197 for three agents, $297 for ten — those come from pre-V2 documentation and no longer match what the pricing page shows. Build your budget from the current page, not from a 2025 blog post.

One more practical thing: CloseBot states outright that there are no refunds. The free plan and the 7-day trial on paid plans exist so you can decide at zero risk instead of asking for money back. If you're testing the Agency plan specifically to evaluate white labeling and rebilling, that trial is where you do it.

## Setup walkthrough: free account to branded client portal

The sequence is shorter than most agency software onboarding, but the order matters.

1. **Create a free account.** No credit card. This gives you 100 replies a month, one agent, and one seat — enough to build a first agent and see whether it books.
2. **Upgrade to the Agency plan** when you're ready to sell. This is what unlocks rebilling and white labeling, including during the 7-day trial.
3. **Connect Stripe.** In Account Settings → Agency → Rebilling, connect your Stripe account and toggle rebilling on.
4. **Set your markup rates.** Decide your per-message, per-seat, and per-MB storage prices. These become your default rates, adjustable per client later.
5. **Build the agent.** Connect a Persona (tone, voice, typo frequency, agent name and image) to a Job Flow built in the drag-and-drop builder. Define the variables your clients will fill in.
6. **White-label the client portal.** Point it at your own domain and apply your colors and logo.
7. **Add the client as a source and enable rebilling** for that specific client, choosing an existing Stripe customer or letting CloseBot create one. They top up their wallet; you set auto-reload if you want.

Most teams get a first agent live the same day. The part that takes longer is deciding what your productized offer actually is — which is an agency problem, not a software problem.

## Limits worth knowing before you sell this

None of the following is fatal, but all of it should be in your head before you promise a client anything.

**You still need a CRM underneath.** CloseBot doesn't connect to Instagram or WhatsApp directly. It takes over the text channels inside your CRM — HighLevel, HubSpot, LeadConnector, custom stacks, or CloseBot's native CRM. That CRM is a separate subscription and a separate line in your cost model.

**No bring-your-own API key.** CloseBot treats this as a security decision and doesn't allow it. On the current business plans the model cost is baked into your base price, which is simpler but also means you can't shave spend by pointing it at a cheaper provider.

**Clients can't build.** By design, and it cuts both ways. It protects you from clients breaking working agents, and it also means any "can you just change this one thing" request lands on your desk. Budget for that.

**Message units can drift.** One message equals one segment, except when you enable the Agent Node's unlimited potential — many tools, unlimited instruction size — where billing switches to token costs and a single reply can consume several segments. If you plan heavy agents, price your markup generously.

**Growth is the compliance door.** HIPAA, quarterly audits, and priority uptime sit behind a custom quote. If you're selling into healthcare or dental, get that quote before you promise a client compliance.

## Who should white label CloseBot, and who shouldn't

It fits you if you already run client accounts on HighLevel or HubSpot, you want a conversational agent that's better than the native one, and you'd rather turn software into a billed service than eat it as overhead. The white-label portal plus Stripe rebilling is close to the most agency-shaped setup in this category — one independent 2026 review calls the white-label and rebilling combination "clearly best in class."

It fits you less well if you're a one-person operation reselling AI to clients you also serve hands-on and can't spare time for agent builds, or if you want an unbranded platform under your own login rather than a branded portal on someone else's app. And if your clients live entirely in Instagram DMs with no CRM in the middle, adding a CRM just to run CloseBot is a bigger project than the white-label question suggests.

If you're in the first group, the cheap way to test the whole thing is a free account and a 7-day agency trial — build one agent, white-label the portal, run a real client's leads through it, and see whether the bookings justify the $397 before you go annual.

Before you check out, one verified discount: CloseBot's own coupon page lists **CLOSEBOT100OFF** for $100 off your first payment, and it applies to both Business and Agency plans. At $397 that's not life-changing, but it's real and it's official.

## Quick answers

**Can I white label CloseBot on the free plan?** No. White labeling and rebilling are Agency-plan features, and the business track doesn't expose those screens at all — including during the agency trial period.

**Does white label mean the whole app carries my brand?** No. Your name, domain, and branding apply to the client portal your clients log into. You and your team still work inside CloseBot.

**How much does it cost?** $397/month monthly, or $331/month equivalent billed at $3,970/year, plus usage at $0.012 per message, $5 per additional seat, and $0.006 per MB of storage per day — all of which you can mark up and rebill.

**Do I need CloseBot's Agency plan to sell AI setting to clients?** If you want the client to see a branded portal and pay you rather than CloseBot, yes. The Agency plan is the only track with re-billing and white labeling built in.
