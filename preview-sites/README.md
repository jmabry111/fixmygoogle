# Mabry Technologies preview sites

Twelve one-page concept sites for prospects without a website. Each is a single self-contained `index.html` (no external files, no build step).

## Deploy to mymabry.com (GitHub Pages)

1. Copy the `previews/` folder into the root of the mymabry.com repository.
2. Merge the line in `robots.txt.example` into the repo's `robots.txt` (create it if missing).
3. Commit and push. Each site is then live at `https://mymabry.com/previews/<folder-name>/`, which is the address printed on each audit.

## Built in

- `noindex, nofollow` on every page, plus the robots.txt rule, so previews never compete with the real business in search.
- A visible "Concept preview by Mabry Technologies" banner and a not-affiliated footer.
- Only facts from each business's public Google listing (name, address, phone, hours, rating, review count, services customers mention). No copied photos or logos.
- LocalBusiness structured data, tap-to-call buttons, and a Google Maps directions link.
- Checked with axe-core against WCAG 2.1 A and AA at desktop and phone widths: no violations.

## When a prospect signs

Move their folder to its own repo, delete the preview banner and footer note, remove the `noindex` tag, add their photos, and point their domain at it with a `CNAME` file.

## Take down

Delete the folder and push. Do this for any owner who asks.
