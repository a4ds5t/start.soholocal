# Built

What is in the page now. The open items and the reasoning behind the choices are in [Development](Development.md). What changed per version is in the [changelog](changelog/README.md).

- Clock: 24-hour, 12-hour and full time with seconds, chosen in Advanced or by clicking the time; the colons stay still. The time in the time zones follows the same choice.
- Date: long or short, chosen in Advanced or by clicking the date. The short date's order follows the browser unless a choice is made (day-month-year, month-day-year or year-month-day). Minimal leaves the date out; Advanced can show it again.
- Time zones: an optional clock icon above the time opens a Time zones window: the local time, up to five zones sorted by UTC offset, and an Edit time zones button that opens the manage panel.
- Weather: optional, off by default. Location from the IP address or a chosen city (choose field only; one active city, replaced on a new pick; cleared from the Weather chip ×). Settings shows a live chip `City - icon temp`. Hover preview and full forecast with icons per hour and per day, the local time of the place, and a Windy link.
- IP details: a button in the basic settings. It shows the last address you asked for, with the city, provider and more; a check button looks it up again. Looked up only on request or when weather needs it.
- Links: with the Links panel on, a control at the top left opens your own links (up to 15). With the panel off it is a Wikipedia button in the UI language. There is no hover-peek.
- Background: the round button at the bottom right cycles through none and each wallpaper switched on in Manage data (Background tab). The button at the bottom left changes the colour in steps, on a phone and on a computer; the colour button can be hidden under Show in Advanced.
- Quote on a phone: under the Ask AI row, not over it.
- Settings shell: **Settings | Data** segment with sidebars (desktop) / list→drill-in (mobile). Quiet filter search thins sidebar sections and content rows (same query across Settings ↔ Data). Settings: General · Show on page · Weather · Clock & date. Data catalogs: Search · AI · Social · Own links · Time zones · Weather · Background · Backup. Ask AI under the bar is icons only; Social and Ask AI rows never show together.
- Weather places: up to five extra places besides your own, shown as chips in the forecast window. Your place stays fixed at the top of Data → Weather; extras reorder with ↑↓ and that order is saved (chips follow it).
- Settings: a basic view (the pages and the privacy note, with Help) and an Advanced view in groups: Weather, Show, Time format, Date, Search, AI shortcuts, Background and Language. Gear icon, Help guide in six languages, Escape closes the top window. The reset buttons sit beside Back to basic settings and ask first.
- AI catalog (Data → AI): one list — built-ins (Claude, ChatGPT, Grok, Gemini, Duck.ai, Lumo, Kagi Assistant, Meta AI) plus custom Add AI. Per item: **In search** (overlay / type + Enter) and **Ask AI row** (up to five under the bar). No separate shortcuts list or Pick service.
- Search: opens in the same tab by default; Advanced can open it in a new tab.
- Pages: Minimal (search, clock and the colour button) and Standard (adds the date, Wikipedia, the colour and wallpaper buttons) presets in the settings, plus Advanced when the choices match neither. They change only the display options; weather and the IP address are never changed by a preset.
- Limits: links (15), time zones (5), AI shortcuts (5) and weather places (5) each show their count, and adding is greyed out when full.
- Privacy: optional features that send data are off by default. Weather and the IP address send data only when switched on or asked for; [Cloudflare Web Analytics](https://developers.cloudflare.com/web-analytics/) collects cookieless, aggregate page views on the live site. A one-line note sits under the IP-address location option in the advanced settings.
- Phones: the bottom controls sit above the browser's bar; the colour and wallpaper buttons are adjusted for touch.
- Import: a choice between Merge (the default; new items added, links matched by address, existing items kept) and Replace. The import reports how many were added, were already there, or were skipped by a limit.
- Language: a choice in Advanced settings (Automatic, or one of six languages). Automatic follows the browser; a choice reloads the page.
