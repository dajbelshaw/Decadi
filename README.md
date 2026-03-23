# Décadi

A daily calendar displaying today's date in the [French Republican Calendar](https://en.wikipedia.org/wiki/French_Republican_calendar), with a background image sourced from Wikimedia Commons for whatever plant, animal, mineral, or tool the day is named after.

![Décadi showing 3 Germinal, An CCXXXIV — the day of Asperge (Asparagus). The screen displays the month name GERMINAL in large serif type, with the day number 3 and decade name Tridi to the right. Below, the French name Asperge and its English translation appear over a Wikimedia Commons photograph of fresh asparagus spears alongside a bowl of asparagus soup.](screenshot.png)

---

## What is the French Republican Calendar?

The French Republican Calendar was introduced during the Revolution in 1793 and used until 1806. It replaced the Gregorian calendar with a rational system of twelve 30-day months, each divided into three ten-day weeks (*décades*). Every day was named for a plant, animal, mineral, or agricultural tool — a deliberate rejection of saints' days in favour of rural, natural life.

The year begins at the autumnal equinox. Each month has a poetic name rooted in the season: *Vendémiaire* (vintage), *Brumaire* (fog), *Frimaire* (frost), *Nivôse* (snow), *Pluviôse* (rain), *Ventôse* (wind), *Germinal* (sprouting), *Floréal* (flowers), *Prairial* (meadows), *Messidor* (harvest), *Thermidor* (heat), *Fructidor* (fruits). Five or six complementary days — the *Sansculottides* — fall at the year's end.

The calendar was named after Décadi, the tenth and final day of each decade: the Republican day of rest.

## How it works

The app calculates the current Republican date from the astronomical autumnal equinox (using the Meeus algorithm), then fetches a background image from [Wikimedia Commons](https://commons.wikimedia.org) for that day's named subject. Images are cached in `localStorage` so only one API request is made per day.

The year count uses the equinox-based astronomical method rather than the historical arithmetic approximation, matching the calendar's original intent.

## Image credits

Background images are fetched at runtime from [Wikimedia Commons](https://commons.wikimedia.org) via the [MediaWiki API](https://www.mediawiki.org/wiki/API:Main_page). Each image is used under its original licence — typically [CC BY-SA](https://creativecommons.org/licenses/by-sa/4.0/) or [CC BY](https://creativecommons.org/licenses/by/4.0/). See the Wikimedia Commons page for any given image for full attribution details.

## Licence

[AGPL-3.0](LICENSE.md)
