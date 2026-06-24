# Summer 2026 Northern Loop — Project Handoff

This doc captures the state of the trip-planning project as of June 24, 2026, for handoff to Claude Code working directly in the repo.

## Repo & deployment

- Repo: `github.com/erik-erik-erik/summer-2026-roadtrip`
- GitHub Pages enabled on `main` branch, root.
- Two pages live:
  - `/` (`index.html` at repo root) — original v1 proposal, **kept as reference**, do not modify
  - `/2026-northern-loop/` (`2026-northern-loop/index.html`) — **current working schedule**, this is what's active

## Trip overview

- **Dates:** Jul 31, 2026 (Fri PM departure) → Sep 13, 2026 (Sun arrival home)
- **Total:** 44 nights, 12 stops, ~54 hr drive, ~4 day buffer at end (home Sun, friend visit Fri Sep 18)
- **Crew:** Erik + Lisa + 8-month-old + 2 dogs
- **Rig:** F-250 + truck camper, ~24-26 ft, ~12 mpg diesel, ~$2,060 mid-estimate fuel
- **Connectivity:** Starlink Roam covers everywhere in BC and PNW with sky view. Tree cover is the only obstacle. Cell coverage is not a constraint.
- **Lisa's work:** New job starts July 20, heavy 4-6 week stretch. Trip schedule is shaped around her working from real basecamps Mon-Fri.

## Final locked schedule

| Date | Day | Stop | Nights | Camping plan |
|------|-----|------|--------|---------|
| 7/31 PM | Fri | Boise / Arrowrock | 1 | Arrowrock BLM dispersed (free) |
| 8/1 | Sat | Yakima River Canyon | 1 | BLM riverside ($15) or L.T. Murray dispersed (free) |
| 8/2 | Sun | Ferry → Lopez arrival | — | ferry day |
| 8/2–8/20 | M-Th | **Lopez Island** | 19 | existing plan |
| 8/21 | Fri | Lopez → Squamish (ferry) | — | — |
| 8/21–8/23 | F/Sa/Su | **Squamish** | 3 | Squamish Valley FSR dispersed (free, Crown land) |
| 8/24 | Mon | Bonaparte Plateau transit | 1 | Crown land dispersed (free) |
| 8/25–8/29 | Tu-Sa | **Revelstoke** | 5 | Boulder Mountain Rd dispersed (free, Crown land) |
| 8/30–8/31 | Su-Mo | **Whiteswan Lake** | 2 | Whiteswan Lake PP FCFS ($25-30) |
| 9/1–9/3 | Tu-Th | **Yoho NP** | 3 | Kicking Horse CG (~$18 with PC 25% off discount) |
| 9/4–9/6 | F/Sa/Su | **Fernie** | 3 | Coal Creek FSR dispersed (free), Mt Fernie PP backup |
| 9/7–9/10 | M-Th | **Glacier east** | 4 | St. Mary CG day-of reservation |
| 9/11 | Fri | Missoula transit + friends | 1 | Lolo NF dispersed (Rock Creek / Blackfoot) |
| 9/12 | Sat | Teton Valley | 1 | Teton Canyon CG shoulder-season FCFS |
| 9/13 | Sun | **HOME** | — | 4-day buffer before 9/18 friend visit |

## Key decisions made (do not relitigate without strong reason)

- **Bugaboos OUT** — dogs prohibited park-wide in BC Parks, can't camp at trailhead lot. Replaced with Whiteswan Lake PP.
- **Manning Park OUT** — deep forest, paid park, not on the dispersed-first ethic. Replaced with Bonaparte Plateau Crown land dispersed (open plateau, Starlink-perfect, free).
- **Helena → Missoula swap** — Lolo NF dispersed + Marshall Mountain MTB + Rattlesnake NRA + reliable friends > Helena's transit-night vibe. Costs ~30-60 min more drive.
- **Schedule flipped from v1** — sprint outbound to Lopez (2 nights vs 14), long Lopez stay, leisurely BC interior return. Driven by Lisa's job starting July 20.
- **No Yellowstone, no Sawtooths, no Wallowas, no Bonneville, no North Cascades** — v1 had these, v2 cut them to honor low-drive-days + real-dwell-time priorities.
- **Two Medicine Glacier CG closed all 2026** (construction) — east-side camping is St. Mary only.
- **Glacier vehicle reservations dropped park-wide for 2026** — no timed entry needed.
- **Parks Canada free admission + 25% off camping June 19 – Sep 7, 2026** — meaningful discount on Yoho.
- **BC Parks moved to 3-month rolling reservation window for 2026** (from 4-month).

## Three open questions (live for Lisa's input)

These are surfaced on the page in the "Open questions" section.

1. **Yoho campground choice** — Working plan: Kicking Horse reservation ($18 with discount, convenient). Alternative: Crown land east of Golden (Blaeberry River FSR, Waitabit Creek Rec Site) — free dispersed but adds 30-45 min each way per day.
2. **Fernie campground choice** — Working plan: Coal Creek FSR dispersed (free, Crown land north of town). Alternative: Mount Fernie PP ($30-43, trails from camp, showers, Rogers LTE).
3. **Lopez length** — Working plan: 19 nights + 4-day end buffer. Alternative: ~14 nights + extend a BC basecamp.

## Pre-trip booking checklist

In order of urgency:

1. **Anacortes ferry** — both directions, especially **return Fri Aug 21** off Lopez
2. **Yoho Kicking Horse** (if going with working plan) — Parks Canada reservation system at `reservation.pc.gc.ca`, opened Jan 22 for whole season, mid-week Tu-Th Sep 1-3 should still have availability
3. **Mount Fernie PP** (only if switching off Coal Creek FSR for Fernie) — `bcparks.ca`, 3-month rolling window opened June 4 for Sep 4 arrival
4. Everything else: FCFS / day-of / dispersed — no advance booking needed

## File architecture (in repo)

```
summer-2026-roadtrip/
├── index.html                          # v1 proposal page (preserve as reference)
└── 2026-northern-loop/
    └── index.html                      # current working schedule (this is what we iterate on)
```

URLs:
- `https://erik-erik-erik.github.io/summer-2026-roadtrip/` — v1
- `https://erik-erik-erik.github.io/summer-2026-roadtrip/2026-northern-loop/` — current

## Design system (preserve when editing)

Visual design is a deliberate editorial / proposal aesthetic. Don't templatize this into a generic site.

- **Fonts:** Fraunces (serif, display + body, opsz variable) and Inter (sans, metadata)
- **Background:** `#f4ede1` warm cream
- **Card background:** `#fbf6ec` slightly lighter
- **Ink:** `#2d2419` deep brown for body
- **Stage colors** (used for map markers, can be referenced elsewhere):
  - `home: #2d2419` deep brown (Park City)
  - `out: #8b3a1d` rust red (outbound sprint: Boise, Yakima)
  - `lopez: #4a6b7a` dusty blue (Lopez)
  - `canada: #3d5240` forest green (Squamish through Fernie)
  - `return: #c47a52` warm orange (Glacier east through Teton Valley)
- **Layout:** alternating destination cards (`.destination` vs `.destination.reverse`)
- **Photos:** 1 main + 2 side, background-image style
- **Map:** Leaflet 1.9.4 with OSM tiles, dashed polyline connecting stops, circle markers colored by stage

## Photo source approach

- All photos are pulled from Google Places via `place_id` lookup
- URLs are stored inline as background-image styles in HTML
- **Known issue:** photos may not load reliably on Erik's view of the v1 page. To be debugged. Possible causes: photos expire, Google Places URL signing, CORS, etc. Worth investigating fresh photo-hosting strategy (self-hosted, Unsplash, etc.) if the issue persists.

## Stops with photo source `place_id` (for refresh if needed)

| Stop | place_id |
|------|----------|
| Boise / Arrowrock | `ChIJbRU6A_7urlQRrAS9MDVHGbI` |
| Yakima River Canyon | `ChIJXWJecqfCmVQR-Z6Z48FBPas` |
| Lopez Island | `ChIJHdXDcROAj1QR4gz38VwqV6Q` |
| Squamish | (from v1, in original index.html) |
| Bonaparte Plateau / Tunkwa Lake PP | `ChIJAQAAAFAygFQRjsm6xG44QSQ` |
| Revelstoke | (from v1) |
| Whiteswan Lake PP | `ChIJV2poNFq8elMRy-psbe-YbzQ` |
| Lussier Hot Springs (related) | `ChIJiU57PLe9elMROnegVt6zRJc` |
| Yoho | (from v1) |
| Mount Fernie PP | `ChIJfQPdw5hsZVMRLKhc8E4LrGY` |
| Glacier east / St. Mary Lake | `ChIJ5_WaQyG6aFMRep8QRW9nvZQ` |
| Missoula | (from v1) |
| Teton Valley | (from v1) |

## Build script (for reference)

I built the `2026-northern-loop/index.html` using a Python script that takes the v1 `index.html` as input and surgically replaces hero, intro, destination cards, tradeoffs, index table, totals, and map JS. Not in the repo currently. If you want reproducible builds going forward, consider committing the build script. Otherwise edit the HTML directly in Claude Code — it's just hand-maintainable HTML.

## Known live tasks for Claude Code to pick up

1. **Image loading bug** — Erik reported images don't reliably load on the v1 page. Top priority to investigate. Test loading from clean browser session, check network tab for failures, check whether place-photos URLs are expiring or being blocked. Solution likely involves either (a) self-hosting photos in repo, or (b) using a different photo service like Unsplash.
2. **Optional: refactor away from build script.** Currently the page is hand-maintainable HTML. If Erik wants to keep iterating on schedule/content, may be worth setting up a small static site generator (Eleventy, Astro, even a basic Jekyll setup) to make adding/reordering stops cleaner. But the current single-file approach is fine if changes are infrequent.
3. **Anchors / nav.** Page lacks anchor links and table-of-contents nav. Could be added if Erik wants easier scroll navigation between sections.
4. **Mobile review.** Built and tested at desktop widths. Mobile should be acceptable (Leaflet is responsive, CSS uses container patterns) but hasn't been thoroughly reviewed.

## Conversational style preferences (for Claude Code)

Erik appreciates:
- Directness over hedging
- Honest pushback when he proposes something with issues
- Surfacing tradeoffs explicitly rather than just recommending
- Citation of specific facts (campground rules, reservation systems, etc.) rather than vague guidance
- Acknowledging his expertise and not over-explaining basics
- The `ask_user_input_v0` multiple choice tool when there are discrete options to pick between

Erik dislikes:
- Sycophancy
- Soft-pedaling concerns
- Excessive caveats
- Made-up details (when in doubt, search or say "I don't know")

## Other context

- Erik's domain on this trip: he's done extensive vehicle prep, knows the rig, knows boondocking. Don't over-explain mechanics.
- Lisa's working: schedule is non-negotiable around her work-week needs Mon-Fri.
- Family: 8-month-old, 2 dogs (good camping dogs). Trail/camp choices must be dog-friendly.
- Erik's project context: this trip planning is part of a broader post-job-separation recovery period. The trip is real and committed. Treat schedule-affecting suggestions with appropriate weight.
