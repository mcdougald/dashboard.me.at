<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset=".github/assets/hero-dark.png">
    <img src=".github/assets/hero.png" alt="dashboard.me.at landing page" width="880">
  </picture>
</p>

<h1 align="center">dashboard.me.at</h1>

<p align="center"><strong>The numbers behind my network: GitHub activity, WakaTime coding hours, Spotify listening, and blog reach.</strong></p>

<p align="center">
  <img src="https://img.shields.io/badge/status-in%20development-171717?style=flat-square" alt="Status: in development">
  <img src="https://img.shields.io/badge/license-source--available-404040?style=flat-square" alt="License: source-available">
  <img src="https://img.shields.io/badge/part%20of-me.at-737373?style=flat-square" alt="Part of me.at">
</p>

<p align="center">
  <a href="#features">Features</a> ·
  <a href="#how-it-works">How it works</a> ·
  <a href="#built-with">Built with</a>
</p>

My coding hours, GitHub activity, listening and blog reach each live in a different place, and none of them tells the whole story alone. I built dashboard.me.at to gather my personal metrics on one page: it pulls live data from GitHub, WakaTime and Spotify, plus view and like counts from my blog, and lays them out as a single scrolling dashboard. It is a personal quantified-self page, not a product, and it is kept out of search indexes.

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset=".github/assets/overview-dark.svg">
    <img src=".github/assets/overview.svg" alt="dashboard.me.at at a glance: coding cadence, GitHub activity, listening history, repository health" width="880">
  </picture>
</p>

## Why

- **One page instead of four tabs**: coding time, repositories, music and blog reach sit side by side, with twelve headline figures up top.
- **Live, not pasted in**: every panel is fed by its source's API rather than typed in by hand, and panel data can be downloaded as CSV or JSON.
- **Fails one card at a time**: a revoked Spotify connection shows one notice instead of breaking every card.

## Features

- **Overview strip**: twelve headline figures (coding time, streaks, repositories, stars, open issues, languages, views, blog likes).
- **Coding cadence**: WakaTime hours for the last 7 and 30 days, active days, average per active day, and the heaviest day.
- **Repository health**: how many repositories are described, licensed, topic-tagged, original, and recently pushed.
- **GitHub metrics**: a contribution calendar, recent pushes, and charts of repository creation, updates, sizes, types, and licenses.
- **Music metrics**: top tracks and artists from Spotify over the last 4 weeks, 6 months, or all time, with list and grid views.
- **Export**: download panel data as CSV or JSON.
- **Mobile-first layout**: a sticky section nav, scroll progress, and print styles.
- **Graceful failure**: a revoked Spotify connection shows one notice instead of failing every card.

## How it works

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset=".github/assets/flow-dark.svg">
    <img src=".github/assets/flow.svg" alt="How dashboard.me.at works: fetch, add reach, summarize, lay out, export" width="880">
  </picture>
</p>

Each section reads its own source: GitHub for repositories and contributions, WakaTime for coding hours, Spotify for listening, and my blog for view and like counts. The overview strip condenses those into twelve headline figures, and the sections below lay out the detail on one page with a sticky section nav. Any panel's data can be exported as CSV or JSON.

## Built with

<p>
  <img src="https://img.shields.io/badge/Next.js-16-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js 16">
  <img src="https://img.shields.io/badge/React-19-171717?style=flat-square&logo=react&logoColor=white" alt="React 19">
  <img src="https://img.shields.io/badge/TypeScript-5-262626?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/Tailwind%20CSS-4-404040?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind CSS 4">
  <img src="https://img.shields.io/badge/Chart.js-Recharts-525252?style=flat-square&logo=chartdotjs&logoColor=white" alt="Chart.js and Recharts">
  <img src="https://img.shields.io/badge/GitHub-API-737373?style=flat-square&logo=github&logoColor=white" alt="GitHub API">
  <img src="https://img.shields.io/badge/WakaTime-API-737373?style=flat-square&logo=wakatime&logoColor=white" alt="WakaTime API">
  <img src="https://img.shields.io/badge/Spotify-API-737373?style=flat-square&logo=spotify&logoColor=white" alt="Spotify API">
</p>

- Next.js 16 (App Router), React 19, TypeScript
- Tailwind CSS 4
- oRPC + TanStack Query
- Recharts, Chart.js, and react-activity-calendar
- GitHub, WakaTime, and Spotify APIs

## Part of the me.at family

dashboard.me.at is one of my [`*.me.at`](https://me.at) apps. They share one design system, account, and app shell. Development happens in a private monorepo; this repository is the project's public-facing home.

## License

Source-available. See [LICENSE](LICENSE).
