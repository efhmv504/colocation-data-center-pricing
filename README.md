# colocation data centers: What They Cost, What's Actually Included, and How to House Your Own Hardware Without Overpaying

Colocation means you keep your servers, rent the building around them. A colocation data center supplies the power, cooling, physical security, and network connectivity; you ship in your own hardware and retain full control over it. The practical questions behind that search are always the same three: what does rack space actually cost per month, what do you get for that money, and which facility deserves your equipment. Sharktech is one option worth a look — it operates five locations (Los Angeles, Las Vegas, Denver, Chicago, and Amsterdam), starts per-server colocation at $79/month, and includes 40 Gbps DDoS protection in every plan instead of selling it as an add-on.

> **Quick pick:** Most people hosting one to three servers need the per-server tier, which starts at **$79/month for 1U with 200W**. Full racks start at $449/month on Sharktech's main colocation page. If that's your range, 👉 [check Sharktech's current per-server colocation pricing](https://bit.ly/SharKtech) and match the power draw to your hardware before ordering.

## What a colocation data center actually does

A colocation facility rents you space — measured in rack units (U), cabinets, or caged areas — plus electricity, cooling, and network access, while you own and maintain the equipment itself. The provider handles the building: redundant power with backup generators, cooling systems, physical access controls, and surveillance. You handle the servers.

The economics are the reason the model persists. Uptime Institute has found that colocation can be 19% to 64% more cost-effective than building your own Tier 2 data center once you factor in cooling, generator backups, redundant networking, and the staff to run all of it. Against public cloud, the math works differently: colocation wins when you already own hardware, run it at steady high utilization, and want direct control over the machines — cloud wins when workloads spike unpredictably or you don't want to touch hardware at all.

## Sharktech's colocation plans and pricing

Sharktech's current public pricing breaks down into per-server space, quarter and full cabinets, and custom cages. Here's what the official pages list:

| Plan | Power | Port speed | Starting price | Billing | Order |
| --- | --- | --- | --- | --- | --- |
| 1U server space | from 200W | GigE, up to 100Gbps | $79/mo | Monthly | [ Order 1U colocation](https://bit.ly/SharKtech) |
| 2U server space | from 280W | GigE, up to 100Gbps | $99/mo | Monthly | [ Order 2U colocation](https://bit.ly/SharKtech) |
| 4U server space | from 450W | GigE, up to 100Gbps | $249/mo | Monthly | [ Order 4U colocation](https://bit.ly/SharKtech) |
| 1/4 cabinet (10U) | from 1200W | GigE, up to 100Gbps | Quoted in portal | Monthly | [ Configure a 10U cabinet](https://bit.ly/SharKtech) |
| 10–42U rack | 1600–5500W | 10–100Gbps | from $449/mo | Monthly | [ See rack colocation pricing](https://bit.ly/SharKtech) |
| Custom cage | Custom | Custom | Itemized quote | Monthly | [ Request a cage quote](https://bit.ly/SharKtech) |

Sharktech's main colocation page summarizes the per-server tier as 1–6U starting at $79/month, with the Denver subdomain page breaking out the 1U/2U/4U price points shown above. The official pages quote everything on a monthly basis.

Two things to verify before you commit. First, pricing varies by location — the same tier is quoted differently across the five cities, and Sharktech doesn't publish a single per-city grid on every page, so treat the figure shown in the ordering portal as the authoritative number for your chosen site. Second, bandwidth allotments are described differently across Sharktech's own pages: the Denver page lists 10TB on a GigE connection, while the main colocation page lists allocations starting at 300TB. That's a meaningful difference, and it's exactly the kind of line item to nail down in writing before you ship hardware. For the full current breakdown, 👉 [see Sharktech's complete plan list and pricing](https://bit.ly/SharKtech).

## What comes included with every plan

The headline inclusion is DDoS protection, and it's worth understanding how Sharktech structures it. Every colocation plan ships with 40 Gbps of DDoS mitigation at no extra charge. The company built its own filtering system rather than reselling a third party's — traffic gets scrubbed locally at each facility using GRE, BGP, and anycast, with attacks mitigated automatically rather than waiting on a human to flip a switch. Upgrades to 100 Gbps are available at order time, and larger capacities are custom-quoted.

Standalone context makes that inclusion concrete: independent DDoS mitigation of similar capacity typically runs from $50 to several hundred dollars per month from dedicated protection vendors. Getting it bundled changes the total-cost picture, especially for game server operators and anything else that attracts attacks as a hobby.

Beyond that, every plan includes:

- **10Gbps to 100Gbps port speeds** on a multi-100-Gigabit redundant network
- **Redundant power and cooling**, including backup generators, across all five locations
- **Enterprise-grade facilities** — Sharktech's colocation space sits inside Equinix, CoreSite, H5 Data Centers, and CrownCastle buildings
- **24/7 on-site technical staff** who can physically reach your hardware, which matters more than it sounds until a server hangs at 3 a.m. and a remote reboot doesn't fix it

Sharktech has been in the DDoS protection business since 2003 and says more than 10,000 businesses use its services overall. Its Trustpilot rating sits at 3.4/5 — based on only 13 reviews, so treat that number as a small sample rather than a verdict. The more granular feedback comes from hosting forums, where a long-running comment sums up the niche well: "If you run game-servers and you need cheap DDoS protection that actually works, you want these guys."

## The line items most colocation articles skip

Most "what is colocation" explainers stop at the monthly rack price and call it done. The bill usually doesn't. These are the extras to price out before committing:

1. **Remote hands.** Sharktech keeps on-site technicians available 24/7 for emergencies, but hands-on work beyond that has an agreed scope and its charges are reviewed before ordering. If your deployment needs regular physical interventions, get that scope priced upfront rather than discovering it per-incident.
2. **Cross-connects.** Direct connections to carriers or other networks inside the facility are a separate charge. Anyone running hybrid setups with specific network providers should count these.
3. **Operating system and panel licenses.** Linux and FreeBSD are free; Windows, cPanel, and DirectAdmin carry licensing fees. On a fleet of machines this adds up.
4. **Extra IP addresses, power, and bandwidth.** Past Sharktech colocation listings have included free IPv4 up to a /27 and a /48 IPv6 block, but going beyond the plan's allocation costs extra, and power overages are the classic surprise on a colocation invoice.
5. **Cancellation mechanics.** Some Trustpilot reviewers noted that canceling means terminating the PayPal subscription yourself. Minor, but worth knowing so you don't pay for a rack you've already emptied.

None of these are hidden — Sharktech's own ordering flow shows power, connectivity, and installation or remote-hands charges for review before you confirm. The point is that the sticker price is the floor, and asking for an itemized quote is the only way to see the ceiling. 👉 [Request an itemized colocation quote from Sharktech before shipping hardware](https://bit.ly/SharKtech).

## Picking a location: five cities, one decision rule

Sharktech runs facilities in Los Angeles, Las Vegas, Denver, Chicago, and Amsterdam. The decision rule is simple: put hardware near the users and networks it serves, and avoid geography that threatens it.

Denver is the location Sharktech has detailed most publicly. The company has promoted it as geologically and meteorologically stable — no earthquake or hurricane exposure — with good connectivity toward Chicago, San Jose, Los Angeles, and Dallas, making it a practical network service point for both US coasts. The Denver facility has been listed with HIPAA, ISO, PCI, and SOC compliance, N+1 or 2N+1 UPS redundancy, N+1 cooling, and a network blend including Zayo, Comcast, and NTT with Noction intelligent routing. If you want to judge the network before committing, Sharktech publishes a Denver test IP at 70.39.65.252 and an Amsterdam test IP at 45.58.188.8 — run your own latency checks from where your users actually sit.

One more location-related freedom worth knowing: Sharktech explicitly states it will never require you to use its network as an upsell. You can bring your own network and IP arrangements via BGP if that's how your infrastructure is built. And because the same tier is priced per city, comparing locations isn't just about latency — it can directly change your monthly bill, so get quotes for two candidate cities before deciding.

## How ordering actually works

Colocation has physical details a web form can't guess, so the process is more consultative than buying a VPS:

1. **Choose a location** — compare the five cities against your users and network requirements.
2. **Specify the hardware** — share rack units, power draw, port requirements, and expected growth. Power draw is the number people get wrong; a 1U server typically starts around 200W, and underestimating it means re-quoting later.
3. **Configure in the portal** — select space, power, and connectivity, then review the full configuration including installation and remote-hands charges before paying.
4. **Coordinate shipment** — arrange shipping and installation details with Sharktech before the equipment leaves your hands.

The last step is worth emphasizing: Sharktech asks customers to share the equipment list and growth plan before shipping, and their team helps match the service to the hardware. Take them up on that. A five-minute conversation about power density prevents the classic mistake of ordering a 1U plan for hardware that pulls 400W.

## Who colocation is wrong for

Honesty time, because colocation isn't the answer to everything:

- **You don't own hardware yet.** Colocation means supplying your own servers. If you're starting from zero, renting a dedicated server from the same provider or using cloud will be faster and cheaper than buying hardware to colocate.
- **You run one low-traffic website.** A shared or VPS plan costs a fraction of even the cheapest 1U slot plus the server you'd feed it. Colocation only makes sense when you have equipment worth housing.
- **You need fully managed everything.** On-site staff handle facilities and emergencies, but patching, backups, and application work stay yours.
- **Your workload is spiky and unpredictable.** Owning fixed hardware for bursty demand wastes money sitting idle; usage-based cloud pricing fits that pattern better.

## FAQ

**How much does 1U colocation cost?**
At Sharktech, 1U starts at $79/month with 200W and a GigE port scalable up to 100Gbps. Other providers and cities price 1U differently, and Sharktech's own per-city rates vary, so treat $79 as the entry point for its five facilities.

**Is DDoS protection really included, or is it an upsell?**
It's included. Every Sharktech colocation plan comes with 40 Gbps of DDoS mitigation for free, upgradeable to 100 Gbps at order time. This is the company's core competence since 2003, and its own customers — including game server operators absorbing 3–8 Gbit attacks regularly, per testimonials Sharktech publishes — rely on it daily.

**How much bandwidth do I get with Sharktech colocation?**
It depends on which page and tier you're looking at: Sharktech's Denver colocation page lists 10TB on a GigE connection, while its main colocation page describes allocations starting at 300TB for the 10Gbps–100Gbps tiers. Because the two official figures differ, confirm the exact bandwidth commitment for your chosen plan and location in the ordering portal before paying — it's the single most important number to get in writing.

**Can I bring my own IP space and network?**
Yes. Sharktech states plainly that it won't require customers to use its network, and BGP sessions with your own arrangements are supported. Cross-connect fees may apply depending on your setup.

**Colocation or cloud — which is cheaper?**
For owned hardware running steadily at high utilization, colocation. Uptime Institute's finding that colocation saves 19–64% versus building your own Tier 2 facility captures the infrastructure side; against renting cloud compute indefinitely, the crossover point usually arrives when hardware is paid for and utilization stays high.

## The short version before you order

One server or two with modest power needs → the 1U/2U per-server tier at $79–99/month does the job, and there's no reason to buy more. Growing past four or five machines → price the 10–42U rack tier, since per-unit economics shift fast. Anything with custom power density, cages, or non-standard networking → get a quote instead of forcing a stock plan. Whatever your path, confirm the bandwidth allocation and power allowance for your specific location in the portal — those two numbers drive the real invoice — and 👉 [configure your Sharktech colocation deployment](https://bit.ly/SharKtech) once the hardware list is final.
