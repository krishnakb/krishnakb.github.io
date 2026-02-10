# Portfolio Website Design

## Overview
Terminal-themed portfolio site for krishnakb.github.io with modern VS Code aesthetic, scroll animations, and interactive timeline.

## Tech Stack
- **Framework**: Astro (static output)
- **Styling**: Vanilla CSS with CSS variables
- **Animations**: CSS transitions + Intersection Observer
- **Fonts**: JetBrains Mono (code), Inter (body)
- **Deployment**: GitHub Pages via GitHub Actions

## Color Palette
```css
--bg: #1e1e1e
--surface: #252526
--border: #3c3c3c
--text: #d4d4d4
--muted: #808080
--blue: #569cd6
--teal: #4ec9b0
--orange: #ce9178
--green: #b5cea8
--purple: #c586c0
```

## Sections

### 1. Hero
- Terminal window chrome (dots, title bar)
- Typewriter effect: `> Hello, I'm Krishna Kanchibhatta`
- Tagline: "Software Engineer @ Spotify | Stockholm"
- Subtitle: "Someone that loves solving problems."
- Nav links styled as terminal commands (clickable)

### 2. Experience (Timeline)
- Vertical timeline on left
- Cards animate in from right on scroll
- Each card shows: title, company (teal), dates (muted)
- Click to expand: tech tags + bullet points
- Jobs:
  - Spotify (Present) - Stockholm
  - Media Transcoding & Orchestration (Feb 2021)
  - Telenor - Voyager Microservices (Oct 2018 - Jan 2021)
  - NetJets Inc. - Trip Planning (Mar 2018 - Sep 2018)
  - Nationwide Insurance (May 2016 - Nov 2017)

### 3. Skills
- Grouped categories with proficiency bars
- Categories: Languages, Frameworks, Cloud, AI Tools, Data
- Visual progress bars (CSS)
- Include: Java, Microservices, System Design, Cloud, Tableau, AI coding tools

### 4. Education
- University of Akron (2014-2016)
- Full tuition waiver
- Terminal-styled card

### 5. Certifications
- Advanced Java Programming - LinkedIn (Mar 2021)
- Systems Expert - AlgoExpert

### 6. Contact
- Icon links: LinkedIn, GitHub, Email
- Terminal prompt styling: `$ connect --with krishna`

## Animations
- Scroll-triggered fade-in for all sections
- Typewriter effect on hero text
- Card expand/collapse transitions
- Subtle hover states on all interactive elements
- Cursor blink on terminal prompts

## File Structure
```
src/
  layouts/Layout.astro
  pages/index.astro
  components/
    Hero.astro
    Timeline.astro
    JobCard.astro
    Skills.astro
    Education.astro
    Certifications.astro
    Contact.astro
  styles/global.css
  data/resume.json
public/
  favicon.svg
.github/
  workflows/deploy.yml
```

## Content Source
- Data from LinkedIn: linkedin.com/in/krishnakanchibhatta
- Name: Krishna Kanchibhatta
- Location: Stockholm, Sweden
- Current: Spotify
- Languages: English, Telugu, Hindi, Swedish (learning)
- Awards: Flexibility Performance Award, Best Trainee Award

## Deployment
- GitHub Actions workflow triggers on push to main
- Builds Astro site
- Deploys to GitHub Pages
- Live at: https://krishnakb.github.io
