# Review of eonai.solutions/en

Reviewed: `/en` (homepage), `/pricing`, `/privacy` (cookie policy). The site has no dedicated tenant, owner or investor pages.

## What the site does well
- **One clear promise.** "Grow your rental portfolio without hiring more admin staff", with Ana (the AI copilot) as the proof.
- **Show, don't tell.** The WhatsApp demo ("Pick a message and watch") pairs the chat with "Meanwhile, in Eon" — the best moment on the page, and the seed of this simulation.
- **Concrete money framing.** The "do this sum" calculator (~€16,800/yr part-time admin vs €3,000/yr Pro) is persuasive and honest about its assumptions.
- **Trust is addressed.** "Money, leases and prices go through a person", automatic deletion of applicant documents, a public sub-processor list.
- **Pricing is simple.** Whole product in every plan; you scale by flats, not features.

## Gaps and opportunities
1. **The page speaks to one persona.** Everything is addressed to the agency. Tenants, owners and investors only appear as supporting cast (chat bubbles, "owners call"), so the *network effect* — the real moat of Eon + Ana — is never shown.
2. **Ana's role as connective tissue is implicit.** The site shows Ana answering a tenant, but not that the same repair becomes an owner-statement line item and a vendor booking. The graph in `index.html` makes that visible.
3. **Investors are invisible until /pricing.** They surface only under "Coming soon → Sales department" (investor links with yield and mortgage on real rents). Marking that flow as a *preview* in the simulation avoids over-promising.
4. **"Human in the loop" is told, not felt.** The approval gate in the simulation turns the "money always goes through a person" line into something you can click.
5. **Language mismatch.** `/pricing` and `/privacy` return English body copy but Spanish meta titles and descriptions (e.g. "Precios — todo el producto en todos los planes"), and `/privacy` metadata is Spanish. Worth aligning `hreflang`, metadata and locale routing (`/en/pricing`).
6. **Anchors point at the root.** CTAs link to `https://eonai.solutions/#demo` and `/#ana-demo` rather than `/en#demo`, which can drop the locale.
7. **Pricing page has a stale-looking strike-through** ("no setup fee (was €99)") that reads oddly next to the €99 plan price; check the copy.
8. **Missing proof.** No customer logos, quotes or measured outcomes (hours saved, arrears reduced). Ana's sample figures are clearly labelled "scripted demonstration", which is good; real numbers would complement them.
9. **Accessibility/contrast.** The extracted brand text colour (#646A82 on black) is low contrast for body copy; worth auditing.

## Where the simulation fits
Place `index.html` (or an embed of it) between "Ana does the work" and the cost calculator, as "See how everyone connects". It gives owners, tenants and investors a seat at a page that today only addresses the agency.
