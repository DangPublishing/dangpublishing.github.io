# Dang Publishing

The home page for Dang Publishing: https://dangpublishing.github.io/

Videos, RunningHub workflows and free browser tools, all in one place.

## Adding or changing a link

Everything on the page comes from one list near the top of `index.html`, marked
**EDIT YOUR LINKS HERE**. To add something:

1. On GitHub, open `index.html` and click the pencil icon to edit.
2. Find the section you want (`tools`, `workflows` or `videos`).
3. Copy an existing `{ ... }` item, paste it inside that section's `items: [ ... ]`,
   and change the words. Keep a comma between items.
4. Click **Commit changes**. The site updates within a minute or two.

Item fields:

| Field | What it is |
|---|---|
| `title` | Name on the card (required) |
| `url` | Where the card goes (required unless it is a YouTube video) |
| `text` | One or two sentences about it |
| `tags` | Small labels, e.g. `['Music', 'Free']` |
| `youtube` | For a YouTube video: the ID after `watch?v=`. The card shows its thumbnail. |
| `date` | Optional, e.g. `'2026-09-26'`. Newer items sort first. |
| `image` | Optional picture for the top of the card, e.g. `'images/my-picture.jpg'`. Upload it to the `images` folder first; wide 16:9 fits best. |

A new section is another `{ id: ..., title: ..., blurb: ..., items: [ ] }` block.
An empty section shows "Coming soon."

To show the YouTube channel button, put the channel link in `channel: { url: '' }`.

## Other pages on this site

- Clip Compare: https://dangpublishing.github.io/video-compare/
- ABC Score Viewer: https://dangpublishing.github.io/abc-viewer/
