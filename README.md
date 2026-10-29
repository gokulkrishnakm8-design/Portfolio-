# Gokul Krishna K M – Portfolio

My own portfolio website for Gokul Krishna K M, a B.Tech Computer Science student at Jawaharlal College of Engineering and Technology (Autonomous). It is a single HTML file with all CSS and JavaScript embedded, so there is nothing to install or build.

## Design

- **Style:** midnight (deep indigo background)
- **Accent colour:** purple
- **Layout:** creative, with a staggered hero name and asymmetric sections
- **Fonts:** Syne (headings) and DM Sans (body), loaded from Google Fonts with system-font fallbacks

## Sections

- **Hero:** name, short intro and links to the project and contact
- **About:** college, programme and current focus
- **Studies:** expandable course list (Programming in C, IT Workshop, Foundations of Computing, Applied Python for AI)
- **Skills:** languages, Python for AI libraries, tools and fundamentals
- **Git and GitHub:** a terminal-style view of the add, commit, push and pull workflow
- **FitDiet:** the college project, with an interactive meal-schedule preview built around a workout time
- **Fitness and nutrition:** training, food timing and consistency
- **Goals:** what comes next
- **Contact:** a message form and optional links

## Features

- Responsive layout with a mobile menu
- Active-section highlighting in the navigation and a scroll progress bar
- Animated star field that reacts to the cursor
- Expandable course details
- Keyboard-visible focus styles
- Respects the system "reduce motion" setting

## Getting started

1. Download `gokul-portfolio.html`.
2. Open it in any modern browser (double-click the file).

An internet connection is only needed for the Google Fonts; the page still works offline with fallback fonts.

## Customising

### Contact links

Open the file and find the `CONFIG` block at the top of the `<script>` tag:

```js
const CONFIG = {
  email: "",      // e.g. "you@example.com"
  github: "",     // e.g. "https://github.com/yourname"
  linkedin: ""    // e.g. "https://www.linkedin.com/in/yourname"
};
```

- Links with a value appear in the Contact section; empty ones stay hidden.
- With an email set, the contact form opens the visitor's email app with the message filled in.
- Without an email, the form copies the message to the clipboard instead.

### Colours

Change the values in the `:root` block at the top of the `<style>` tag:

| Variable | Purpose |
| --- | --- |
| `--bg`, `--bg2` | Page and panel backgrounds |
| `--pur`, `--pur2` | Main and light purple accents |
| `--ink`, `--mute` | Main and secondary text |

### Content

Edit the text directly in the HTML. Each section has an `id` (`about`, `studies`, `skills`, `git`, `fitdiet`, `fitness`, `goals`, `contact`) that matches a navigation link.

## Hosting

Because it is one static file, you can publish it for free:

- **GitHub Pages:** push the file to a repository, rename it to `index.html`, then enable Pages in the repository settings.
- **Netlify or Vercel:** drag and drop the file or connect the repository.

## Notes

- The FitDiet meal preview is a demonstration of the idea only. It does not give nutrition advice.
- Goals and fitness text are written as a starting point; edit them to match your own plans.

## Tech

HTML, CSS and vanilla JavaScript. No frameworks or dependencies.
