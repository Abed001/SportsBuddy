# SportsBuddy Design System (final)

Responsive web app, mobile-first. Dark charcoal hero band on every page, white rounded cards overlapping it.

## Colors
Charcoal #1E1F24 (hero, navbar, footer), Charcoal Soft #2A2B31, Lavender #A99BFF (featured card, active tab), Lime #D6F55B (navbar "Create run" and landing CTAs only), Ink #14151A, Muted #6B6F7A, Page #F3F3F5, Success #16A34A on tint #DCFCE7, Danger #DC2626.
Rules: lime is a fill with Ink text, never text. No lavender text on white. Text on lavender is Ink.

## Typography
Syne 700 for headings. Space Grotesk 700 for all numbers (distance, pace, stats, counts). Inter for body and UI. Min text size 12px.

## Shape
Cards 24px, buttons and chips pill, inputs 16px, soft shadow only.

## Components
- Navbar: logo left, Browse / My Runs in a dark pill switcher center, lime "Create run" + avatar right. Logged-out: "Log in" outline pill + lime "Sign up".
- Info pills: charcoal fill, white text.
- Join button: charcoal fill, white text, pill. Joined: light green tint, green text, check icon. Leave: red outline.
- Run card: white, one category of info only (date/time, title, distance + pace, location pill, avatars with +N, action).
- Stat tiles: Space Grotesk number, small muted label.
- Footer: charcoal, 3 links left, copyright right.

## Don't
No gradients, no rotated cards, no neon glow, no fields outside the data model (see schema).