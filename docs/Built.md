# Built

What is in the page now. The open items and the reasoning behind the choices are in [Development](Development.md). What changed per version is in the [changelog](changelog/README.md).

- Clock: 24-hour, 12-hour and full time with seconds, chosen in Advanced or by clicking the time; the colons stay still. The time in the time zones follows the same choice.
- Date: long or short, chosen in Advanced or by clicking the date. The short date's order follows the browser unless a choice is made (day-month-year, month-day-year or year-month-day). Minimal leaves the date out; Advanced can show it again.
- Time zones: an optional clock icon above the time opens a Time zones window: the local time, up to five zones sorted by UTC offset, and an Edit time zones button that opens the manage panel.
- Weather: optional, off by default. Location from the IP address or a chosen city. Hover preview and full forecast with icons per hour and per day, the local time of the place, and a Windy link.
- IP details: a button in the basic settings. It shows the last address you asked for, with the city, provider and more; a check button looks it up again. Looked up only on request or when weather needs it.
- Links: a globe at the top left opens a Links window with the permanent links as logos in a row (Wikipedia, Google, Apple, Facebook, X, Instagram, Microsoft, GitHub, Reuters) and your own links below; up to 15 of your own. A Manage data button in that window opens the full manage panel, where your own links are edited. Hovering the globe shows your own links only. The button can be switched off. With Own links off it is a plain Wikipedia button that opens Wikipedia directly; the Minimal page uses that.
- Background: the round button at the bottom right cycles through none and each wallpaper switched on in Manage data (Background tab). The button at the bottom left changes the colour in steps, on a phone and on a computer; the colour button can be hidden under Show in Advanced.
- Quote on a phone: under the AI shortcuts, not over them.
- Settings shell: one fixed window with a left sidebar (General, Search, AI, Social, Links, Time zones, Weather, Background, Advanced, Backup). Catalogs that used to live in Manage data sit here; on a phone the sidebar becomes bottom tabs plus a menu. The links globe, time zones clock and forecast Edit places open the matching pane. Ask AI under the bar is icons only; Social and Ask AI rows never show together.
- Weather places: up to five extra places besides your own, shown as chips in the forecast window.
- Settings: a basic view (the pages and the privacy note, with Help) and an Advanced view in groups: Weather, Show, Time format, Date, Search, AI shortcuts, Background and Language. Gear icon, Help guide in six languages, Escape closes the top window. The reset buttons sit beside Back to basic settings and ask first.
- AI shortcuts: a checklist of eight services (Claude, ChatGPT, Grok, Duck.ai, Lumo, Kagi, Meta AI, Gemini); up to five, your own shortcuts included. Each has a monochrome icon; a shortcut's icon is checked once when it is saved. Links open in a new tab by default.
- Search: opens in the same tab by default; Advanced can open it in a new tab.
- Pages: Minimal (search, clock and the colour button) and Standard (adds the date, Wikipedia, the colour and wallpaper buttons) presets in the settings, plus Advanced when the choices match neither. They change only the display options; weather and the IP address are never changed by a preset.
- Limits: links (15), time zones (5), AI shortcuts (5) and weather places (5) each show their count, and adding is greyed out when full.
- Privacy: optional features that send data are off by default. Weather and the IP address send data only when switched on or asked for; [Cloudflare Web Analytics](https://developers.cloudflare.com/web-analytics/) collects cookieless, aggregate page views on the live site. A one-line note sits under the IP-address location option in the advanced settings.
- Phones: the bottom controls sit above the browser's bar; the colour and wallpaper buttons are adjusted for touch.
- Import: a choice between Merge (the default; new items added, links matched by address, existing items kept) and Replace. The import reports how many were added, were already there, or were skipped by a limit.
- Language: a choice in Advanced settings (Automatic, or one of six languages). Automatic follows the browser; a choice reloads the page.
