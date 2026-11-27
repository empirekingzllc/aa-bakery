# Bakery concept-demo template

Plain static HTML and CSS for pitching a small bakery or home-treats business. There is no build step and no framework. GitHub Pages serves this repository from the `main` branch root, including at `https://empirekingzllc.github.io/aa-bakery/`. Asset URLs are relative, so the same files work at that project path and inside a subfolder.

This repository is public, so the photos and files in it can be browsed on github.com.

The page is a concept demo. The notice at the top and in the footer stays exactly:

> Unofficial concept demo by Automation Architects — not the business’s official website.

The order form is demo-only. It checks the fields in the browser and then shows “Demo only — nothing was sent.” It has no `action`, and the script does not call the network or write to storage. The fields stay disabled when JavaScript is off.

## Clone it for a prospect

1. Copy the root `index.html` and the `assets/` folder into a new hard-to-guess folder, for example `p-` plus 8 random hex characters (`p-3f9a1c2b`).
2. Replace every `{{placeholder}}` in that copy, including `{{BUSINESS_NAME}}`, `{{CITY}}`, `{{IG_HANDLE}}`, `{{TREAT_1}}`, `{{TREAT_2}}`, `{{TREAT_3}}`, `{{NOTICE_DAYS}}`, and `{{DELIVERY_FEE}}`.
3. In the script, set `MIN_LEAD_DAYS` to the same lead time you write into `{{NOTICE_DAYS}}`. Keep placeholder text inside the script a valid JavaScript string.
4. Swap photos only for images whose rights you can document. Record provenance (title, author, license, source URL) with that copy. Update each `alt` text and the footer photo credit to match the new files.
5. Keep the demo notice and the demo-only form.
6. Keep `<meta name="robots" content="noindex, nofollow, noarchive">` on the page.
7. Do not link prospect folders from the root page, the template, or this README.

A live order form needs a real form handler approved by Joshua.

## robots.txt

`robots.txt` is:

```
User-agent: *
Disallow: /
```

For a project Pages site, GitHub serves `robots.txt` only from the user-site root (`https://empirekingzllc.github.io/robots.txt`), not from this project. The `noindex` meta tag is the real protection. `.nojekyll` is at the repository root so Pages serves the files as they are.

## Stock photos

The placeholder photos are CC0 (public domain). Sources:

- `assets/bg_desktop.webp` and `assets/bg_mobile.webp` — crops of [Macarons Pixabay.jpg](https://commons.wikimedia.org/wiki/File:Macarons_Pixabay.jpg), Pixabay user pexels, CC0. The wide crop is the desktop background; the tall crop is the smaller-screen background.
- `assets/g_macarons.webp` — the same [Macarons Pixabay.jpg](https://commons.wikimedia.org/wiki/File:Macarons_Pixabay.jpg), CC0.
- `assets/g_donuts.webp` — [Donuts in a box with different types.JPG](https://commons.wikimedia.org/wiki/File:Donuts_in_a_box_with_different_types.JPG) by Tomwsulcer, CC0.
- `assets/g_oatmeal.webp` — [Oatmeal cookies on a plate.jpg](https://commons.wikimedia.org/wiki/File:Oatmeal_cookies_on_a_plate.jpg) by Evan Prodromou, CC0.

CC0 deed: https://creativecommons.org/publicdomain/zero/1.0/
