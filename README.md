# Auction Platform: Legal & Launch Guide

> **Disclaimer:** This guide is research and general information, not legal advice. Laws change and differ by country. Before launching, get a written legal opinion from a qualified lawyer in your launch country (gaming and e-commerce law). Research date: October 2026.

---

## 1. Summary

| Question | Short answer |
|---|---|
| Is the model legal? | **Likely legal in many markets** (especially the UK) if the winner is decided by bidding rules, not luck, and fees are small, clear and refundable before the start. Not guaranteed everywhere. |
| Best first market | **United Kingdom** |
| Biggest legal risk | Being classified as gambling or a lottery (paid entry + prize + chance) |
| Biggest practical risk | **Payment providers** refusing or closing the account |
| Must do before launch | UK legal opinion, approved payment provider, clear terms, anti-bot protection |

---

## 2. How the platform works

1. **Join:** The user pays a **participation fee of about 1% of the item's value** to reserve a spot. Each auction has a limited number of spots.
2. **Cancel anytime before the start:** **full refund**. If an auction never fills, everyone is refunded automatically.
3. **Notification:** When all spots are filled, participants are notified of the start time.
4. **Free bidding:** Each click raises the price by a fixed small amount. Bidding costs nothing.
5. **Starting price:** Bidding starts at a set price (recommended around 50% of value).
6. **End of auction:** When the timer runs out, or when the price reaches the **cap of 80% of the item's value**, so no one pays more than 80% of retail.
7. **Winner:** The highest bidder when the timer ends. If the cap is reached, a **clear, non-random tie-break** decides (for example, the participant who placed the most bids).
8. **Winner pays** the final price **plus shipping**. No buyer fee.
9. **Losers** get **20% of their participation fee back as credits**, which can be used on the platform or withdrawn.
10. **All rules are shown simply before joining.**

---

## 3. The core legal question: auction or gambling?

Most countries define gambling or a lottery with **three elements**:

| Element | In this model |
|---|---|
| **Payment** (consideration) | Yes, the participation fee |
| **Prize** | Yes, the item below retail |
| **Chance** | **Should be NO.** The winner must be decided by bidding, not luck |

If all three are present, it is usually gambling and needs a license. The design must make sure **the third element is absent**.

### Why this model is much safer than a "penny auction"

Penny auctions (pay per bid) have been heavily criticised and, in some countries, banned:
- **Germany:** authorities and courts treated penny auctions as **illegal gambling**.
- **USA:** several operators faced class actions (QuiBids, BigDeal.com, DealDash), and Washington State shut one site down for fake bidding.
- **UK:** the Gambling Commission **does not consider penny auctions gambling** under the Gambling Act 2005.

This platform differs in important ways:

| Feature | Penny auction | This platform |
|---|---|---|
| Cost per bid | Paid | **Free** |
| Entry cost | Often none, but bids add up | **Small fee (~1%)** |
| Refund before start | No | **Full refund** |
| Maximum price | Can go above retail | **Capped at 80% of value** |
| Losers | Lose everything spent | **Get 20% back as credits** |

### Features that keep it legal

1. **Non-random winner rule.** Never use a random draw or "fastest click wins" at the cap. Use a written rule such as "most bids placed" or "highest bid when the timer ends."
2. **Small, transparent fee.** About 1% of the value, called a "participation fee," shown before joining.
3. **Full refunds** before the start, and automatic refunds if an auction doesn't fill.
4. **No fake bidders or bots** run by the platform. This is illegal in most markets.
5. **Anti-bot protection** for users, so the "most bids" rule can't be won by scripts.
6. **Honest marketing.** Never promise users they will win or save money. Show the full cost.

### Remaining grey areas

- **Losers keep only 20% of the fee.** Strict regulators may still argue users pay mainly for a chance. The small 1% fee reduces this risk. Raising the refund (for example to 50%) would reduce it further.
- **Withdrawable credits** may need an e-money or payment license depending on the country (see Section 6).
- **Each country** applies its own consumer, auction and tax rules.

---

## 4. Country-by-country overview

| Region | Risk | Notes |
|---|---|---|
| **United Kingdom** | **Low** | Gambling Commission says penny auctions are not gambling under the Gambling Act 2005. This model is safer than a penny auction. Consumer law and payment rules still apply. |
| Rest of EU (France, Spain, Italy, etc.) | Low–Medium | No clear rulings found. Strict EU consumer law: transparent pricing, refunds, no misleading claims. |
| Germany | Medium–High | Courts treated penny auctions as illegal gambling. Avoid at launch. |
| Netherlands | Medium–High | Very strict enforcement against unlicensed games of chance (large fines). Avoid at launch. |
| USA | Medium | State-by-state gambling laws, frequent class actions. Lower risk for this model than for penny auctions, but needs state-level advice. |
| Brazil | Medium | Strong consumer code (refund rights). Games of chance outside authorized frameworks are an offense. Auctions may require a registered auctioneer. |
| Mexico | High | Any betting-like activity needs a SEGOB permit, rarely granted. Stripe also prohibits penny auctions there. |
| Tunisia | High | State monopoly on games of chance, and a 2026 bill proposes a total ban on online games of chance with prison penalties. |

---

## 5. Recommended launch market: United Kingdom

**Why the UK:**
- Clearest legal position from the gambling regulator.
- A UK limited company can be registered online quickly, and founders don't need to live there.
- Large, card-friendly market with strong investor credibility.

**Expansion path after the UK:**
1. UK (launch and prove the model)
2. Selected EU countries (avoiding Germany and the Netherlands at first)
3. Selected US states, after state-level legal advice
4. Other markets once legal opinions are in place

---

## 6. Payments

### Key finding
- **Stripe** lists **"bidding fee auctions"** as **prohibited** (under gambling). It also prohibits penny auctions in Mexico and games of skill or sweepstakes with a prize. Even though this platform charges an entry fee rather than a per-bid fee, Stripe could still classify it as prohibited. **Don't build on Stripe without written approval.**
- **PayPal** requires **pre-approval** for any activity with an entry fee and a prize. Apply via aup@paypal.com with contact details, the website URL and a business summary.

### Recommended approach
1. Get the UK legal opinion first. Providers will ask for it.
2. Apply to **2–3 providers at the same time**, describing the model honestly: *"Auction marketplace, free bidding, small refundable participation fee, winner chosen by highest bid."*
   - **PayPal** (pre-approval)
   - **Adyen** or **Checkout.com** (case-by-case review)
   - **High-risk merchant providers** (e.g. Nuvei, Paysafe, Trust Payments): higher fees, more stable for this type of business
   - *Policies change; confirm each provider's position directly before signing.*
3. Keep a **backup provider** active from day one.

### Credits and user money
- Keep credits as **your own store credit**, usable only on the platform (providers treat this more favourably than third-party stored value).
- Make **withdrawals go back to the original payment card** as refunds where possible.
- Hold user money in a **separate account**.
- Ask the lawyer whether withdrawable credits require an **e-money license** in the UK.

---

## 7. Business model and economics

**Revenue sources:**
- The **winner's final price**
- The **part of participation fees not returned** (80% of each loser's fee)

**Example:** item worth 1,000, bought for 900, 1% fee (10), 50 participants, losers get 20% back.

| Final price | Fees kept (49 × 8) | Total in | Profit |
|---|---|---|---|
| 800 (cap) | 392 | 1,192 | +292 |
| 600 | 392 | 992 | +92 |
| 500 | 392 | 892 | −8 |

**Notes:**
- With a 1% fee, fees alone rarely cover the item cost unless there are a very large number of participants. The **winner's payment** must cover most of the cost.
- A **starting price** (around 50% of value) protects against auctions ending too low.
- **Buying items below retail** (wholesale, partnerships) increases margin.
- Use the Auction Profit Calculator to test different values.

---

## 8. Launch checklist

| # | Step | Status |
|---|---|---|
| 1 | Register a UK limited company | ☐ |
| 2 | Hire a UK lawyer (gaming + e-commerce): written opinion on the model | ☐ |
| 3 | Draft terms and conditions, auction rules, refund and privacy policies | ☐ |
| 4 | Apply to 2–3 payment providers with the legal opinion attached | ☐ |
| 5 | Open a business bank account | ☐ |
| 6 | Confirm whether credits need an e-money license | ☐ |
| 7 | Build anti-bot protection and the tie-break rule | ☐ |
| 8 | Publish a clear "How it works" page | ☐ |
| 9 | Data protection compliance (UK GDPR) | ☐ |
| 10 | Soft launch with a small number of auctions | ☐ |
| 11 | Collect real data and pitch investors | ☐ |

---

## 9. Possibilities and alternative models

If a market or payment provider rejects the core model, these versions lower the risk further:

| Variant | Change | Effect |
|---|---|---|
| **Full credit back** | Losers get 100% of the fee back as credits | Almost removes the "paying for a chance" argument |
| **Higher partial refund** | Losers get 50% back | Lower risk, still earns from fees |
| **Buyer's fee model** | No entry fee; winner pays a small commission | Works like a standard online auction house |
| **Free entry route** | Offer a free way to join some auctions | Weakens the "payment" element in some countries |
| **Bid-to-buy** | Losers can use their fee toward buying the item at a fixed price | Feels more like shopping |
| **B2B / brand partnerships** | Brands supply items for promotion | Lower item cost, marketing revenue |

---

## 10. Is it legal?

**In the UK, this model is likely legal**, provided that:
- the winner is decided by clear bidding rules, not luck,
- the fee is small, transparent and refundable before the start,
- there are no fake bidders and there is protection against bots,
- payments go through an approved provider,
- marketing is honest, and terms are clear.

**In stricter countries** (Germany, Netherlands, Mexico, Tunisia), the risk remains higher and specific legal advice is required before entering.

**The final confirmation must come from a written legal opinion** in the launch country. That opinion also helps with payment provider approval and investor confidence.

---

## Sources

- [UK Gambling Commission – Penny auctions](https://www.gamblingcommission.gov.uk/public-and-players/guide/page/penny-auctions)
- [Stripe – Restricted and prohibited businesses](https://stripe.com/us/restricted-businesses/)
- [PayPal – Acceptable Use Policy](https://www.paypalobjects.com/webstatic/en_NO/ua/pdf/acceptableuse.pdf)
- [World Online Gambling Law Report – German penny auction cases](https://www.imgl.org/wp-content/uploads/2023/02/woglr_august_2013_penny_auctions_0.pdf)
- [Cato Institute – Should penny auctions be regulated under gaming law?](https://www.cato.org/regulation/summer-2014/should-penny-auctions-be-regulated-under-gaming-law)
- [Markou – Penny auctions and EU consumer law](https://plemochoe.euc.ac.cy/entities/publication/63fab7a3-27a1-42f3-a92e-16a3e11837dd)
- [Racklify – Are penny auctions legal?](https://racklify.com/encyclopedia/are-penny-auctions-legal-consumer-protection-compliance-and-best-practices-for-ecommerce/)
- [FTC – Penny auction warning](https://www.ftc.gov/news-events/press-releases/2011/08/ftc-cautions-consumers-pitfalls-penny-auctions)
- [Washington AG – PennyBiddr](https://atg.wa.gov/news/news-releases/pennybiddr-agrees-cash-out-and-refund-consumers-under-agreement-washington)
- [Courthouse News – BigDeal.com class action](https://www.courthousenews.com/?p=269886)
- [Wikipedia – QuiBids](https://en.wikipedia.org/wiki/QuiBids.com)
- [next.io – Dutch regulator fine](https://next.io/?p=139992)
- [Canaltech – Leilão de centavos (Brazil)](https://canaltech.com.br/colunas/golpe-oportunidade-leilao-centavos/)
- [Advennt – Online gaming in Mexico](https://advennt.com/jurisdictions/online-gaming/mexico/)
- [Business News – Tunisia gambling bill 2026](https://businessnews.com.tn/2026/01/20/jeux-de-hasard-et-paris-en-ligne-des-deputes-proposent-un-durcissement-radical-du-cadre-legal/1383910/)
