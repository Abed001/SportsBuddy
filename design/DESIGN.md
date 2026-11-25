# SportsBuddy Design System

Web app (responsive, mobile-first) that helps people find running buddies. Not a native app.

## 1. Brand
- Name: always "SportsBuddy" (one word, capital S and B). Never "Club", "Collective", "Hub" or "Run Collective".
- Tone: energetic, clean, athletic. Not corporate.
- Logo: simple walking-figure icon in a lime circle, next to the wordmark "SPORTSBUDDY".
- Footer copyright: "© 2026 SportsBuddy".

## 2. Colors
| Token | Value | Use |
|---|---|---|
| primary | #d6f55b | Main buttons, highlights, joined states |
| primary-hover | #c4e645 | Button hover |
| primary-content | #131418 | Text on lime |
| charcoal-dark | #131418 | Page background |
| charcoal | #1e1f24 | Dark surfaces |
| charcoal-light | #282a30 | Raised dark elements |
| charcoal-border | #32353d | Dark borders |
| lavender-card | #e8e5f8 | Tags, soft highlights |
| lavender-tag | #5b46e5 | Tag text, active tabs |
| surface | #faf8ff | Light sections |
| surface-container-lowest | #ffffff | Cards |
| on-surface | #1a1b21 | Main text on light |
| on-surface-variant | #6b7280 | Secondary text |
| outline | #e5e7eb | Borders on light |
| success | #22c55e | Joined / confirmed |
| danger | #ef4444 | Leave run, errors |

Rule: dark page background with white cards. Lime is the only action color. Use at most one lime element per card.

## 3. Typography
- Headings and hero text: Syne, weight 800 (700 for smaller headings).
- Numbers and stats (distance, pace, duration, counts): Space Grotesk, weight 700.
- Body and UI text: Inter, 400 / 500 / 600.
- Wordmark in the navbar: regular bold sans-serif, 16px, one line. Not the wide display font.
- Minimum text size: 12px for footers and captions, 14px for body, 16px for form inputs.

## 4. Shape and spacing
- Cards: 24px radius (rounded-2xl). Inner tiles: 12 to 16px.
- Buttons, pills, badges, avatars: fully rounded.
- Page side padding: 16px on mobile.
- Touch targets: at least 44px tall. Primary buttons: full width, 52px tall on mobile.

## 5. Components
- **Navbar (mobile):** one line. Left: logo and wordmark. Right: bell and avatar on main screens. On inner screens (Run Detail, Create Run, Sign up, Log in): back arrow on the far left, then logo and wordmark. Never wrap, clip or overlap.
- **Bottom nav (mobile):** Browse, My Runs, center "+" (lime, create run), Profile. No other tabs in MVP.
- **Run card:** white, 24px radius. Date pill on top, title in Syne, photo, distance and pace chips (Space Grotesk), location line, avatar stack with "X of 10 joined", lime "Join" pill (grey "Joined" when joined).
- **Stat tile:** large Space Grotesk number, small label under it.
- **Form card:** white rounded card on the dark page, bold Syne heading, labeled inputs with visible borders, full-width lime submit button, link to the other auth screen.
- **Inputs:** empty by default with placeholders ("Your name", "you@example.com", "Enter your password"). Never prefilled.
- **Tabs / filters:** pills. Active pill is lavender with lavender-tag text.

## 6. Screens in scope (MVP)
Landing, Sign up, Log in, Browse Runs, Run Detail (including joined state), Create Run, Profile (including My Runs: Joined / Created).

## 7. Out of scope for now (Phase 2)
Rankings and leaderboard, badges, chat, court or event booking, payments, multiple sports. Do not add these to MVP screens.

## 8. Content rules
- No invented stats or user counts (no "1,000+ runners").
- No promo or filler lines, no leaked prompt text, no third-party logins (Strava, Apple).
- Maximum 10 runners per run. Never show more than 10 joined.
- Use the same mock data on every screen.

## 9. Mock data (canonical)
- **Sunrise Waterfront Tempo:** Sat, Oct 24 · 6:30 AM to 7:15 AM. Hudson River Park, Pier 26. 8.5 km, 5:15 /km, 45 min. Host: Marcus Vance, lead pacer, 142 runs hosted. 6 of 10 joined (7 of 10 after joining). Participants and paces: Marcus 5:15, Elena 5:10, Jordan 5:20, Sarah 5:15, David 5:12, Maya 5:20.
- **Central Park North Loop:** Sun, Oct 25 · 8:00 AM. Central Park, Engineers' Gate (90th St). 10.2 km, 5:30 /km. 4 of 10 joined.
- **Bridge to Bridge 10K:** Thu, Oct 29 · 7:00 PM. Brooklyn Navy Yard, Building 77. 10.0 km, 5:00 /km. 7 of 10 joined.
- **Profile user:** Alex Rivera. 38 runs joined, 12 hosted, 14 weeks streak.

## 10. Accessibility
- Text contrast at least 4.5:1 (dark text on lime, white text on charcoal).
- Visible focus states on all interactive elements.
- Icon-only buttons need an aria-label.
- Every input has a visible label.