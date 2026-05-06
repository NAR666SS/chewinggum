# JAWFUEL — Meta Ads Launch Playbook (India)
**Budget tier: ₹500–1,200/day testing**
**Goal: validate that paid Instagram traffic in India will buy a ₹599 tin of premium chewing gum**

This is the working plan. I'll be driving Meta Ads Manager via the Chrome extension once you're logged in — this doc is the spec I'm executing against. Read it once so we're aligned, then we go.

---

## 0. What you have to do (I can't do these for you)

1. **Log into Meta Business Suite** at business.facebook.com in Chrome — same tab as the Claude in Chrome extension.
2. **Have a payment method on the ad account** (debit/credit card or UPI auto-pay). Meta won't let me launch a campaign without one attached.
3. **A Facebook Page for JAWFUEL.** Required even for IG-only ads. Takes 2 minutes — Pages → Create New Page → name it JAWFUEL, category "Health/Beauty," skip the rest.
4. **Connect your Instagram Business account.** If your IG isn't a Business account: IG app → Settings → Account type → Switch to Professional → Business → category "Health/Beauty."
5. **Pick a payment processor for the website.** Razorpay is the obvious one in India — we'll set this up after the campaign goes live, but ideally before.

I'll handle everything else inside Ads Manager via the browser.

---

## 1. The campaign I'm about to build

```
CAMPAIGN: JAWFUEL — Sales — Test 1
└── Objective: Sales (Purchase optimization)
    ├── Ad Set A: "Looksmax Broad — Tier 1 Male 18-28"
    │   └── Daily budget: ₹400
    │   └── 3 ads (Creative 1, 2, 3)
    └── Ad Set B: "Gym + Aesthetic Interests"
        └── Daily budget: ₹400
        └── Same 3 ads
```

Total: **₹800/day = ~₹11,200 over 14 days.**

Same 3 creatives in both ad sets so Meta can find the winning audience × creative combo.

---

## 2. Targeting (this is the bit I need you to confirm)

### Ad Set A — Broad
- **Locations:** Mumbai, Delhi, Bengaluru, Pune, Hyderabad, Chennai, Gurgaon, Noida, Ahmedabad, Kolkata (Tier-1 metros only — that's where premium DTC actually converts)
- **Age:** 18–28
- **Gender:** Men
- **Languages:** English, Hindi
- **Detailed targeting:** EMPTY (broad — Meta's algorithm uses your pixel to find buyers; better than interest stacks at this budget)
- **Placements:** Instagram only — Feed, Reels, Stories, Explore. No Facebook. No Audience Network.

### Ad Set B — Interest-targeted
- **Same location / age / gender / language**
- **Detailed targeting (any of):**
  - Bodybuilding
  - Gym
  - Skincare for men
  - Men's fashion
  - Self-improvement
  - Andrew Tate (interest)
  - Hamza (search if available)
  - Looksmax (likely won't exist as an interest — that's fine)
  - Nike, Adidas (lifestyle proxies)
- **Same placements**

### Who NOT to target
- Tier-2/3 cities right now — shipping logistics + cash-on-delivery RTO rates will eat your margin during testing. Add them once you have a working funnel.
- Women — your messaging is jaw/looksmax-coded. Different ad later.
- Outside India — different ad account, different shipping math.

---

## 3. The 3 creatives you need to shoot

You film these on your phone. **Do not pay for production.** Phone footage outperforms studio on Meta because it doesn't look like an ad. Each is 9:16 vertical.

### Creative 1 — "The Lecture Chew" (POV / native)
**15s vertical Reel.**
- 0–2s: You in a classroom or library, slight smirk to camera. Caption: **"POV: chewing your 4th piece in class"**
- 2–6s: Hand slides JAWFUEL tin out of pocket under desk, slow open.
- 6–10s: You pop a piece, jaw flexes. Side-profile shot.
- 10–13s: Caption: **"0 smell. 0 sugar. 6 hour chew."**
- 13–15s: Tin spinning, end card: **jawfuel.in**
- **Audio:** Trending Hindi/English lo-fi or a quiet looksmax sound from Reels.

### Creative 2 — "30-Day Side Profile" (testimonial)
**20s vertical, two clips spliced.**
- 0–3s: Black screen, big text **"Day 1."** → cut to neutral side-profile selfie.
- 3–6s: **"Day 30."** → same side-profile, chin tucked, mouth closed. Same shirt + lighting.
- 6–10s: Voice-over: "All I did was chew this." Hand holds tin.
- 10–14s: Quick cuts — pop piece, slow-mo jaw clench, accent green flash.
- 14–18s: On-screen: **"Mastic gum. 4× harder than Center Fresh. Built for the masseter."**
- 18–20s: End card with site URL.
- **Audio:** Slow build, drop on Day 30 reveal.

### Creative 3 — "Resistance Test" (educational hook)
**12s vertical.**
- 0–2s: Two pieces of gum on black surface. **"This is what you've been chewing →"** points at Center Fresh.
- 2–4s: Squish it — flattens.
- 4–6s: **"This is JAWFUEL →"** point at JAWFUEL piece.
- 6–8s: Press it — barely moves. **"4× harder."**
- 8–10s: Voice-over: "Your jaw is a muscle. Train it like one."
- 10–12s: Tin appears, end card.

### Ad copy (paste with the videos)

**Variant A:**
```
the gum that gave me a side profile.

• 4× harder than Center Fresh
• 0 sugar / 0 calories / 0 smell
• 5–8 hour chew
• 100% mastic from Chios

launch price: ₹599/tin → jawfuel.in
free shipping over ₹999
```

**Variant B:**
```
chewed this through every class for a month. friends started asking what changed.

JAWFUEL — premium mastic gum. 0 sugar, 0 smell, all-day chew.
30-day jaw-back guarantee.

→ jawfuel.in
```

**Variant C:**
```
your masseter is a muscle. you've been training it with sugar.

JAWFUEL is mastic resin from Chios — the highest-resistance natural chew on earth. 4× harder than commercial gum, 5–8 hour chew, scentless.

₹599. ships pan-India. → jawfuel.in
```

---

## 4. Budget & bidding

- **Daily total:** ₹800 (₹400 per ad set)
- **Optimization event:** Purchase if pixel has data. For first 5–7 days with no pixel data, optimize for "View Content" or "Add to Cart," then switch.
- **Bid strategy:** Highest volume (default). No cost cap until we have benchmarks.
- **Schedule:** Run continuously, not on a schedule.
- **Currency:** INR. Set this on the ad account before first launch — it can't be changed later without creating a new account.

---

## 5. What to watch (only metrics that matter)

| Metric | Healthy at ₹400/ad set | Bad |
|---|---|---|
| **CPM** (per 1k impressions) | ₹120–₹400 | >₹600 |
| **CTR** (link click rate) | >1.5% | <1% |
| **CPC** | ₹6–₹25 | >₹40 |
| **Add-to-cart rate** | >5% of clicks | <2% |
| **CAC** (cost per purchase) | <₹599 (= breakeven on first sale) | >₹800 |
| **ROAS** | 1.5–3.0× at this scale | <1.0 |

**Rules:**
- Don't touch anything for the first 3 days. Meta needs ~50 events per ad set to exit "learning phase."
- If CTR < 1% after 2 days → creative problem, not targeting. New videos.
- If CTR fine but no purchases after ₹4,000 spent → site/checkout problem.
- Don't bump budget more than 20%/day on a winning ad set; bigger jumps reset learning.

---

## 6. The 14-day decision tree

**Day 1–3:** Launch. Don't touch.

**Day 4–7:** First read. 1+ purchase at <₹800 CAC = signal, let it ride. Otherwise pivot the worst creative.

**Day 8–14:** Optimize.
- Working → duplicate winning ad set, +50% budget, broaden audience, build retargeting.
- Marginal → tighten the offer. Try "Buy 2 get 10% off" or lower the free-shipping threshold to ₹699.
- Dead (0 purchases at ₹8,000 spent) → pause. Don't dump more in. Diagnose creative or product-market fit before relaunch.

---

## 7. Honest expectations

At ₹800/day × 14 days = **₹11,200**. Realistic:

- **Best case:** 12–25 purchases, ROAS 1.5–2× → validated, scale.
- **Median case:** 2–6 purchases → marginal, iterate creative for round 2.
- **Worst case:** 0–1 purchases → first-launch normal. Most Indian DTC brands need 3–5 creative iterations to find one that scales.

The first ₹11,200 isn't profit. It's information: which audience clicks, which creative converts, what your real CPM is in this niche, where the funnel leaks. Spend the next ₹20,000 on what you learned.

---

## 8. The honest product caveat

Mastic gum has *some* research behind masseter hypertrophy, but the "jaw transformation" is mostly marketing. Real outcome: modest visible muscle definition over 4–8 weeks of daily use. The 30-day refund clause in the FAQ exists so unhappy customers can leave gracefully without it eating margin or generating bad reviews. Honour it without fighting people — it's cheaper than a 1-star Google review.

---

## TL;DR — what we're about to do together

1. You: log into business.facebook.com, attach Claude in Chrome to that tab.
2. Me: build the campaign per Section 1, plug in the targeting from Section 2, configure budget per Section 4.
3. You: upload the 3 video creatives when prompted (you'll need to shoot these — see Section 3).
4. You: paste in the 3 copy variants from Section 3.
5. Me: hit "Publish."
6. Both: walk away for 72 hours. Don't touch.

If you don't have the videos shot yet, we can launch with placeholder static images of the tin (worse but not zero) and swap to the real videos once you have them.
