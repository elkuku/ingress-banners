# My Ingress banners

A page of the Ingress mission banners I have done: my mission medals from Ingress, matched with
[Bannergress](https://bannergress.com), with a map of where each banner starts.

This repository (`ingress-banners`) is made and filled by the
[Ingress Banners app](https://github.com/elkuku/ingress-banners-android) — there is nothing to edit by hand.

## How it works

1. In the app, sign in with GitHub: it creates this repository from
   [ingress-banners-template](https://github.com/elkuku/ingress-banners-template) and turns on GitHub Pages.
2. Sign in to Bannergress in the app: it saves your done list here (`done.json`).
3. In Ingress, open your agent profile, tap the arrow next to the mission medals and take screenshots
   while you scroll down (about half a screen each, wait until the pictures have loaded). Share them
   to the app: it puts them in `inbox/`.
4. The workflow stitches the screenshots (`capture/medals.jpg`), matches every medal row with your done
   list by picture and publishes the page. Medals it can't match for sure are marked **To check**:
   pick the banner in the app (saved in `corrections.json`).

The page is at `https://<your GitHub name>.github.io/ingress-banners/`.

**Privacy:** the page is public and shows on a map where you did banners. Delete the repository to
remove it.

## Files

| File | |
|---|---|
| `config.json` | Your agent name |
| `inbox/` | New screenshots from the app (emptied by the workflow) |
| `capture/medals.jpg` | Your stitched mission medals |
| `done.json` | Your Bannergress done list |
| `corrections.json` | Medals you matched by hand in the app |
| `notes.json` | Optional notes per banner (Bannergress id → text) |

The build itself is in [elkuku/ingress-banners-tool](https://github.com/elkuku/ingress-banners-tool).
