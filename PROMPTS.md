# Prompts Used: SeatSense

**Tool:** Claude (Anthropic)
**Event:** Prompt Wars, theme: Smart Campus & Student Life

## Prompt: Building SeatSense

> Build SeatSense, a single-file web app (HTML, CSS and vanilla JavaScript, no frameworks) that helps college students find a free seat in the library before they walk there.
>
> **Problem:** Students waste time walking to a full library or searching for a seat in the right zone.
>
> **Core features:**
> - A floor map of 48 seats arranged in tables, split into a Quiet zone and a Group zone
> - Seat states: free, taken and "your seat", shown with colour and a pattern so colour is not the only signal
> - Zone filter buttons that dim the other zone
> - A live occupancy percentage at the top with a plain-language label
> - Tap a free seat, choose 30 minutes, 1 hour or 2 hours, and reserve it
> - A banner with a live countdown and a Release seat button
> - A "Best time to visit" bar chart by hour with the quietest remaining hour highlighted
> - A demo-speed switch where 1 hour passes in 1 minute
>
> **Behaviour:** Simulate other students arriving and leaving every few seconds. If the seat I selected is taken, tell me. Only one reservation at a time.
>
> **Design:** A calm teal and slate palette, a bold geometric heading font, mobile-first, light and dark mode, visible keyboard focus, reduced-motion support.
>
> **Technical:** Save my reservation in localStorage inside try/catch. Announce changes in an aria-live region. Everything in one index.html.
>
> **Out of scope:** Login, backend, real sensors.
>
> Also write a short README.md.

**Result:** A working `index.html` and README.

## Follow-up fix
> The duration dropdown reset to 1 hour every time the map refreshed. Remember the chosen duration across refreshes.

**Result:** The selected duration is now stored in a variable and restored on every render.
