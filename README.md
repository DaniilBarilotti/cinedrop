# CineDrop — let cinema surprise you

Can't decide what to watch? Pick a themed case, spin the reel, and CineDrop drops your next film,
series or anime.

**[Open the live site → cinedrop-beta.vercel.app](https://cinedrop-beta.vercel.app)**

![CineDrop home page with tonight's wild card case](screenshots/home.jpg)

## Features

- **Case opening** — choose a case and spin the cinema reel; it stops on one title, your pick for
  tonight. Quick opening and Skip animation are there when you are in a hurry.
- **43 themed cases** — 22 movie cases (genres, decades, themes, actor and director ensembles),
  8 series cases, 8 anime cases and 5 animation cases. Each case holds up to 1,500 titles, and
  every case cover is a fan of real posters from that case.
- **Discover** — browse more than 12,800 films, search by film, actor or director, filter by
  genre and sort. New releases are added automatically every day.
- **Series and anime** — search the live [TVmaze](https://www.tvmaze.com/) and
  [AniList](https://anilist.co/) catalogs; series show their IMDb rating where IMDb has one, and
  anime listings only include titles that have actually aired.
- **Ratings with sources** — every rating shows where it comes from (IMDb, TMDb, TVmaze or
  AniList) and its snapshot date.
- **Accessible and responsive** — keyboard friendly, screen-reader announcements for the result,
  reduced-motion support, and a layout built for phones as well as desktops.
- **Sound effects** — optional reel sounds, off by default.

## Screenshots

| The reel lands on your pick | Discover the catalog |
| --- | --- |
| ![The cinema reel stopped on the chosen film](screenshots/case-opening.jpg) | ![The Discover page with search and filters](screenshots/discover.jpg) |

<p align="center"><img src="screenshots/phone.jpg" alt="CineDrop on a phone" width="300"></p>

## Tech stack

| Area | Technology |
| --- | --- |
| Framework | [Next.js 16](https://nextjs.org/) (App Router), React 19 and TypeScript |
| Styling | [Tailwind CSS 4](https://tailwindcss.com/), [shadcn/ui](https://ui.shadcn.com/) components and [Inter](https://rsms.me/inter/) |
| Icons | [Lucide](https://lucide.dev/) |
| Data | Film datasets derived from TMDb, [Stremio Cinemeta](https://github.com/Stremio/stremio-addon-sdk) for new releases, IMDb ratings and posters, TVmaze for series and AniList for anime |
| Hosting | [Vercel](https://vercel.com/) |

## Data

The film catalog combines the TMDb / Udacity dataset, The Movies Dataset and a 250-film demo
collection. Cinemeta is checked daily for new releases and current IMDb ratings, so the catalog
keeps growing without a redeploy. Series come from TVmaze (CC BY-SA) with IMDb ratings where
available; anime come from AniList. Posters fall back to an alternate source when the main image
fails. Ratings are snapshots, not live rankings.

This product uses TMDB API-derived datasets but is not endorsed or certified by TMDB. Film imagery
and metadata belong to TMDB and the respective rights holders.

## Source code

The source code is private. I'm happy to walk through it — get in touch through my GitHub profile.
