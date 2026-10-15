# bandwagonhost hosting: every plan and price compared, the refund fine print most reviews skip, and how to pick between budget KVM and CN2 GIA

BandwagonHost hosting splits into two products that share a control panel and almost nothing else: budget KVM servers from $49.99/year, and China-optimized CN2 GIA servers running from $169.99/year up to $89.99/month for Hong Kong. The brand behind it, operated by IT7 Networks Inc. and known as 搬瓦工 in Chinese-speaking communities, has been selling self-managed VPS since 2012. Hardware is solid across both lines. The route is what changes, and the route is what you're paying for at the top end.

That split is where buyers either save money or waste it. Order a budget box expecting premium China routing, or pay GIA prices for a blog that never touches a Chinese visitor, and you've bought the wrong product. Below is every currently listed plan with verified pricing, what the 30-day refund actually covers (narrower than the headline suggests), and a simple way to match a tier to what you're hosting.

> **Quick take:** if you just need a cheap, reliable dev box, the **20G KVM at $49.99/year** is the pick — roughly $4.17/month. If your traffic touches mainland China, the CN2 GIA-E tier from $169.99/year is the one long-time users point to, and it sells out often enough that availability, not price, is the real constraint. [👉 see BandwagonHost's full plan list and current prices](https://bwh81.net/aff.php?aff=77528) Every plan includes a 30-day refund window, a 99.9% uptime guarantee, and manual renewal only — the company never charges your card automatically.

## What BandwagonHost actually is

Short answer: a budget VPS specialist that owns everything it sells. IT7 Networks buys and runs its own enterprise-grade servers — Intel Xeon across most nodes, with newer AMD EPYC machines and NVMe RAID-10 storage live in New York — and owns its own IP space. Nothing is rented from a third party. That's why a hardware failure at a cheap competitor can leave you down for hours while this fleet stays boring and stable.

A few operational habits matter before you buy:

- Every VPS node is checked for failure and overload every minute, and the network gets weekly security audits.
- Setup is instant after payment. All plans ship with full root access, tun/tap VPN support and instant rDNS.
- The service is strictly self-managed. Support covers infrastructure and network problems; your application is your problem, and the terms of service ask you to confirm you can run a Linux server unassisted.

That last point filters out plenty of people on its own. If you want someone else to fix your web server config, this is the wrong store.

One external data point: ServerPicks' 2026 deep-dive scored the platform 8.4/10 overall, with speed (8.5) and value (8.9) as its strongest marks and support (7.9) the weakest. That matches a company investing in network and hardware rather than hand-holding.

## Every BandwagonHost plan and price, listed

The core lineup is six KVM plans, all on a 1 Gbps port with RAID-10 SSD storage. The two smallest sell as multi-month prepay; the four larger ones are pure monthly.

| Plan | RAM / CPU | Storage | Transfer | Price | Buy |
| --- | --- | --- | --- | --- | --- |
| 20G KVM | 1 GB / 2 cores | 20 GB SSD | 1 TB/mo | $49.99/yr | [ Get the 20G plan](https://bwh81.net/aff.php?aff=77528) |
| 40G KVM | 2 GB / 3 cores | 40 GB SSD | 2 TB/mo | $52.99 per half-year (or $99.99/yr) | [ Get the 40G plan](https://bwh81.net/aff.php?aff=77528) |
| 80G KVM | 4 GB / 4 cores | 80 GB SSD | 3 TB/mo | $19.99/mo | [ Get the 80G plan](https://bwh81.net/aff.php?aff=77528) |
| 160G KVM | 8 GB / 5 cores | 160 GB SSD | 4 TB/mo | $39.99/mo | [ Get the 160G plan](https://bwh81.net/aff.php?aff=77528) |
| 320G KVM | 16 GB / 6 cores | 320 GB SSD | 5 TB/mo | $79.99/mo | [ Get the 320G plan](https://bwh81.net/aff.php?aff=77528) |
| 480G KVM | 24 GB / 7 cores | 480 GB SSD | 6 TB/mo | $119.99/mo | [ Get the 480G plan](https://bwh81.net/aff.php?aff=77528) |

Things the table doesn't show:

- The 20G annual plan amortizes to about $4.17/month. The 40G half-year works out to roughly $8.83/month with a shorter commitment.
- The 40G plan also has a $99.99/year option if you'd rather prepay for twelve months than six.
- Monthly plans cost more per month but let you walk away any time. If you're testing an idea, that flexibility is worth the premium.

Above the basic line sit the China-optimized tiers, where the routing — not the specs — is the product:

| Line | Route | From | Best for | Buy |
| --- | --- | --- | --- | --- |
| CN2 GIA-E | Premium CN2 GIA via LA | $169.99/yr | China-facing sites | [ Check CN2 GIA-E availability](https://bwh81.net/aff.php?aff=77528) |
| LA E-Commerce | CN2 GIA | $49.99/quarter | China commerce on a budget | [ See E-Commerce pricing](https://bwh81.net/aff.php?aff=77528) |
| ECOMMERCE SLA | Triple-carrier, 99.99% SLA | $239.99/yr | Mission-critical workloads | [ See SLA plan pricing](https://bwh81.net/aff.php?aff=77528) |
| Osaka CN2 GIA | CN2 GIA/CTGNet both ways, 1.5 Gbps port | $49.99/mo | Japan entry with China routing | [ See Osaka pricing](https://bwh81.net/aff.php?aff=77528) |
| Hong Kong / Tokyo GIA | Premium GIA, lowest latency | $89.99/mo | Real-time traffic to China | [ See Hong Kong pricing](https://bwh81.net/aff.php?aff=77528) |

[👉 grab the 20G KVM plan at $49.99/year](https://bwh81.net/aff.php?aff=77528) if the budget line covers you — everything else on this page is about deciding whether it doesn't.

## Is the CN2 GIA routing worth the premium?

If your users are in mainland China, yes. This routing is the entire reason BandwagonHost has outlasted a decade of cheaper rivals. Premium tiers ride China Telecom's CN2 GIA route, and independent tests put real-world latency around 158ms to the mainland with near-zero packet loss even during evening peak, when standard international routes can lose 30% or more of packets at the same hours.

The engineering behind that number is real. The network aggregates 8×10Gbps CN2 GIA links across two Los Angeles datacenters, peers directly with Google, Apple and ByteDance, and at the USCA_9 Los Angeles node hands China-bound traffic to three carriers at once: Telecom's CN2 GIA, China Mobile's CMIN2 and Unicom's premium route. CN2 GIA transit can cost as much as $120 per megabit commercially — a full gigabit of it would bill around $100,000 a month in some markets. BandwagonHost buys that capacity wholesale and resells it in VPS-sized slices, which is also why the top tiers keep selling out.

If your audience is elsewhere, skip the premium math entirely. The budget line's international routing is ordinary, so judge it as an ordinary cheap VPS and spend accordingly.

[👉 check CN2 GIA tier prices and availability](https://bwh81.net/aff.php?aff=77528) before planning around a specific China tier, since stock moves.

## The fine print that decides whether you'll like it

Two headline policies — a 30-day refund and 99.9% uptime — come with conditions that most reviews gloss over. They matter.

The refund has teeth. Thirty days, yes, but it excludes renewals, blacklisted IPs, and any account that has used more than 10% of its monthly transfer quota. Requesting a refund also takes down every service on that account. Two practical consequences: don't burn half your bandwidth in week one and then change your mind, and don't consolidate all your servers under one login if you might want money back on one of them.

Nothing auto-renews, and that cuts both ways. BandwagonHost doesn't store your payment details, so surprise charges are impossible. The flip side is that renewal is your job, and an invoice left unpaid for seven days suspends the server. Set a calendar reminder the day you buy. One consolation: promo codes apply to renewals too, not just the first purchase.

Bandwidth is suspended, never billed. Hit your transfer quota and the port goes dark until the next cycle. No overage invoices, but no warning cushion either — size the plan honestly.

DDoS protection is nullrouting. Under attack, the target IP gets blackholed: the attack stops, and so does your server, briefly. Services with heavy DDoS exposure should plan for that.

Some uses are banned outright. BitTorrent, cryptocurrency mining, Tor and open proxies are all prohibited, and CPU is throttled on a one-hour average, so sustained maxing-out gets dialed back.

[👉 start with a plan inside the 30-day refund window](https://bwh81.net/aff.php?aff=77528) and test the route from your own connection before the clock runs out.

## The SLA pays real credits (on the plans that include it)

In November 2025, BandwagonHost added a formal SLA to plans that expressly include it — 99.99% monthly uptime, compensated in prepaid time on a published schedule:

| Downtime in a calendar month | Service credit |
| --- | --- |
| Over 4 min 32 s, under 10 min | 12 hours of prepaid time |
| 10–59 minutes | 72 hours |
| 60–119 minutes | 120 hours |
| 120–239 minutes | 240 hours |
| 240–419 minutes | 360 hours |
| 420 minutes or more | One full month |

The mechanics: claims must be filed within 90 days of the end of the calendar month, in a ticket titled "SLA Service Credit" — a general support request doesn't count. Credits come as prepaid time, capped at one month per month, and the exclusion list is broad (maintenance, your own misconfiguration, DDoS mitigation, upstream networks). Read it as compensation mechanics with actual numbers behind them, not insurance. Plans without the SLA carry the baseline 99.9% uptime guarantee.

## KiwiVM and the migration trick most people miss

Every plan runs through KiwiVM, the company's in-house panel. It looks dated and doesn't try to be cPanel, but it covers the whole job: start/stop, OS reloads from 20+ templates, snapshots, rDNS management, an emergency console, usage stats and API access.

The feature worth building a purchase around is free datacenter migration. You can move a running VPS between locations without reprovisioning or losing data — something most hosts at this price don't offer at any price. Standard lines can switch among nine locations: Vancouver, San Jose, three separate Los Angeles datacenters, Fremont, New York, Amsterdam, Dubai, Osaka and Tokyo. The premium China tiers unlock more, within a total footprint of 19+ regions across the US, Canada, Japan, Hong Kong, the Netherlands and the UAE.

The practical play: buy the cheap plan, measure the route from your own connection, and move the machine if Los Angeles turns out to be the wrong door. Cheap insurance for a decision most people make blind.

Payments run through Alipay, UnionPay, PayPal and major credit cards. That combination is rare at this end of the market and a big part of why the brand grew by word of mouth in communities where Stripe-only checkout is a wall.

## When BandwagonHost is the wrong pick

Honest version: it's a poor fit for three kinds of buyers.

Bandwidth-hungry workloads burn through quota fast here, and overage means suspension, not a bigger bill. For hourly-billed global developer clouds, Vultr starts at $2.50/month. For absolute floor pricing with no China requirement, RackNerd's recurring annual specials run $10.98–11.99/year — roughly a quarter of BandwagonHost's entry cost, in exchange for one-to-three-year commitments. And if you need premium China routing with more location choices than this lineup offers, DMIT is the main alternative, from $36.9/year.

What none of those three replicate is the combination of owned hardware, nine-location free migration and a decade-long CN2 GIA track record. The trade is deliberate: you give up hand-holding, DDoS absorption and generous bandwidth to get route quality at this price.

## BandwagonHost FAQ

**Does BandwagonHost auto-renew my plan?**
No. It never stores your payment details or charges automatically. You get reminders, you pay when you choose, and an unpaid invoice suspends the server after seven days.

**Is BandwagonHost managed hosting?**
No, and it doesn't pretend otherwise. Support handles infrastructure and network issues only.

**Is it good for reaching mainland China?**
Yes — it's one of the community standard-bearers. Expect roughly 158ms latency with near-zero packet loss at peak on the CN2 GIA tiers.

**What payment methods does it accept?**
Alipay, UnionPay, PayPal and major credit cards.

**What happens if I exceed my monthly transfer?**
The port is suspended until the next billing cycle. You are never billed for overage.

**Why is CN2 GIA-E so often out of stock?**
CN2 GIA capacity is genuinely scarce and expensive to hold. When the tier is live, that's the time to buy.

## Picking a plan in one pass

- Cheap box for dev, blogs and learning → **20G KVM, $49.99/year.** Free migration means you can relocate later if your needs change.
- China-facing site or API → **CN2 GIA-E from $169.99/year**, stock permitting.
- China routing on a tighter budget → the **LA E-Commerce line from $49.99/quarter**.
- Real-time traffic where milliseconds matter → **Hong Kong GIA from $89.99/month**.
- Contractual uptime requirements → **ECOMMERCE SLA from $239.99/year** at 99.99%.

Before you pay, two things. Confirm which line you actually need, since the route and not the specs is the difference. Then set that renewal reminder and check whether a current promo code applies — it will carry over to every renewal.

[👉 open BandwagonHost's plan page and lock in your pick](https://bwh81.net/aff.php?aff=77528)
