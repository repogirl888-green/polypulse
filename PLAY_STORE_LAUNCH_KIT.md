# PolyPulse — Google Play Launch Kit

Everything needed for the Play Store listing, ready to paste. Target: launch week of July 20, 2026.

---

## 1. Store Listing Copy

**App name (30 char max):**
PolyPulse: Market Tracker

**Short description (80 char max):**
Live prediction market trends. See what the crowd really thinks — in real time.

**Full description (paste as-is):**

The pulse of the prediction markets — in your pocket.

PolyPulse is a live dashboard for prediction markets: places where thousands of people back their forecasts about real-world events with real money. Elections, awards shows, sports, entertainment, world events — PolyPulse shows you what the crowd collectively believes will happen, updated every 60 seconds.

WHAT YOU GET

★ Live Ticker — a scrolling marquee of the hottest markets and their current prices, jazz-club-marquee style

★ Price = Probability — every market shows its YES price in cents. A market at 67¢ means the crowd gives it a 67% chance. Simple as that.

★ Three Lenses — sort by Hottest (where money is moving today), Ending Soon (about to resolve), or Toss-Ups (markets near 50¢ where the crowd is truly split)

★ Instant Search — filter every market as you type. Try "election," "Grammys," or "box office."

★ Probability Bars — see the YES/NO split visualized on every card

★ Fast & Light — no account, no sign-up, no ads, no tracking. Opens instantly.

WHO IT'S FOR

Curious minds who want to know what's really expected to happen — not what one pundit thinks, but what a crowd with skin in the game believes. Great for news junkies, trivia lovers, entertainment watchers, and anyone learning how prediction markets work.

THE FINE PRINT

PolyPulse is an independent information tool. It displays publicly available market data and does not accept bets, wagers, deposits, or payments of any kind. It is not affiliated with, endorsed by, or sponsored by Polymarket. Nothing in this app is financial advice.

A Galsinger Media lab project. Built with love (and vanilla JavaScript) in Newark, NJ.

---

## 2. Category & Contact

- **App category:** News & Magazines (alt: Finance — News & Magazines reads less gambling-adjacent to reviewers)
- **Tags:** prediction markets, trends, news, data
- **Contact email:** galsingermedia@gmail.com
- **Website:** https://repogirl888-green.github.io/polypulse/
- **Privacy policy URL:** https://repogirl888-green.github.io/polypulse/privacy.html

---

## 3. Data Safety Form (answer exactly this)

- Does your app collect or share any of the required user data types? → **No**
- Is all of the user data collected by your app encrypted in transit? → N/A (no data collected)
- Do you provide a way for users to request that their data is deleted? → N/A (no data collected)

Result shown to users: "No data collected / No data shared." (True — no accounts, no analytics, no SDKs.)

---

## 4. Content Rating Questionnaire (IARC) — answer honestly

Most answers are No (no violence, no sexual content, no profanity, no user-generated content, no location sharing).

**The one that matters:** there are questions about gambling. Answer truthfully:
- Does the app contain simulated gambling? → **No**
- Does the app facilitate real-money gambling? → **No** (it takes no bets, holds no money)
- Does the app contain references to gambling / provide information related to real-money wagering? → **Yes** (it displays odds from a real-money prediction market and can link out to it)

Expect a **Teen or Mature** rating because of the reference. That's fine and normal for odds/market-data apps. Never answer dishonestly to get a lower rating — that's the #1 cause of app takedowns.

**Decision to make before submitting (flag for Deborah):** whether v1 keeps the tap-through links to polymarket.com or removes them for the store build. Removing outbound links to the real-money platform makes the review cleaner and the app purely informational. Links can return in an update later. RECOMMENDATION: launch v1 without outbound links, add them post-review if desired.

---

## 5. Visual Assets Checklist

| Asset | Spec | Status |
|---|---|---|
| App icon | 512×512 PNG | ✅ Have it (icon-512.png) |
| Feature graphic | 1024×500 PNG/JPG | ⬜ To make (gold pulse + wordmark on plum — can generate) |
| Phone screenshots | 2–8, min 320px, 16:9-ish | ⬜ Take from live site on phone: ticker view, card grid, Toss-ups view, search in action |
| Optional: 7" & 10" tablet screenshots | improves listing | ⬜ Optional, skip for v1 |

Screenshot tip: use the live PWA installed on the phone (full-screen, no browser bar) for clean captures.

---

## 6. Account & Packaging Steps (launch week)

1. **D-U-N-S check** — see if Galsinger Media LLC already has a D-U-N-S number (dnb.com lookup, free). Org account = no 12-tester requirement. If no D-U-N-S, request one (free) OR launch under individual account and run the 14-day closed test — decide based on timing.
2. **Create Play Console developer account** — play.google.com/console, $25 one-time.
3. **Add assetlinks.json to the repo** — tiny file PWABuilder provides; goes at /.well-known/assetlinks.json so the Android app opens without a browser bar.
4. **Package with PWABuilder** — pwabuilder.com → paste https://repogirl888-green.github.io/polypulse/ → Generate Android package (.aab). No code rewrite; it wraps the live PWA.
5. **Create the app in Play Console** → upload .aab → paste all listing copy above → complete Data Safety + Content Rating + target audience forms.
6. **Submit for review.** First-app reviews typically take a few days to a week.

---

## 7. Pre-Submission Legal Check (one Deborah consult)

- PolyPulse name clearance (USPTO search done 7/17 — only hit is DEAD/ABANDONED in Class 016 ✅ — confirm common-law/Polymarket-proximity comfort)
- Store listing language re: Polymarket references (independence disclaimer already included above)
- Outbound-link decision (Section 4)

---

*Prepared July 17, 2026 · PolyPulse · Galsinger Media*
