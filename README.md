# Engrace Financial Solutions website

The website for Engrace Financial Solutions, rebuilt from the original Wix site as a plain HTML/CSS site. It has no build step and no dependencies, so it can be hosted for free on GitHub Pages, Netlify or Vercel.

## What's in here

| Path | Page |
|---|---|
| `index.html` | Home |
| `about/` | About, team and partner professionals |
| `preserve-it/` | Preserve It |
| `protect-it/` | Protect It |
| `pass-it-on/` | Pass It On |
| `blog/` | Blog list, with one folder per post |
| `contact/` | Contact form, address and map |
| `css/style.css` | All styling (colours are set at the top of the file) |
| `js/main.js` | Mobile menu |
| `images/` | All images, resized for the web |
| `wealth-accumulation/`, `copy-of-family/`, `copy-of-business/`, `news-updates/`, `post/` | Redirects from the old Wix addresses, so existing links and Google results keep working |

## Editing text

Open the page's `index.html` and change the text between the tags. For example, the home page headline is in `index.html` inside `<h1>…</h1>`.

## Previewing on your computer

Double-click `index.html` to open it in a browser. For links to behave exactly as they will online, run this in the project folder and open http://localhost:8080:

```bash
python3 -m http.server 8080
```

## Contact form setup (required before going live)

A static site can't send email by itself, so the form uses [Formspree](https://formspree.io) (free for up to 50 messages a month):

1. Sign up at formspree.io and create a form. Use the email address you want messages sent to.
2. Copy the form ID. It looks like `xyzabcd`.
3. In `contact/index.html`, replace `YOUR_FORM_ID` with that ID.

## Adding a blog post

Copy one of the folders in `blog/`, rename it, and edit the title and text. Then add a card for it to `blog/index.html`.
