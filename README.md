# Kaepora

<img src="https://raw.githubusercontent.com/iamjason/kaepora-site/main/assets/icon.png" width="128" height="128" alt="Kaepora's carved wooden owl icon">

**Your browsers. One friendly switch.**

Kaepora is a small macOS menu bar app that sends links to the browser you choose. Set Kaepora as your default browser once, then use the owl in your menu bar to decide where links open.

## Choose where a link goes

- **Always** — pick your usual browser and keep using it until you change your selection.
- **Next link** — send one link to a different browser, then return to your usual choice.
- **15 min** — switch browsers temporarily, with a countdown in the menu.
- **Hold Option** — choose a browser at your cursor. Use the arrow keys and Return, or Escape to cancel. The modifier is configurable.

Kaepora discovers installed browsers, remembers your selection, and can also forward local HTML documents. If a browser is unavailable, it asks you to choose another. It does not keep a browsing history.

## Availability

Kaepora is **experimental** and requires **macOS 15 or later**. Visit the [website](https://iamjason.github.io/kaepora-site/) for availability and the latest download. Published builds are signed with Developer ID and notarized by Apple.

This repository contains Kaepora's public information, artwork, and Compendium manifest. The application source is maintained separately.

## The woodland family

Named for Kaepora Gaebora, the owl who offers guidance in *Ocarina of Time*, Kaepora joins Deku and Korok in the [Hyrule Compendium](https://iamjason.github.io/hyrule-compendium-site/).

The Compendium discovers this repository through the `hyrule-tool` topic and uses [`hyrule.json`](hyrule.json) for its listing. Published releases will appear in the Compendium on its next refresh.

## Website publishing

This is a static GitHub Pages site served from `main` at the repository root, matching Deku and Korok. `.nojekyll` keeps the HTML and CSS unchanged.

From the separate Kaepora application checkout, `./kaepora update-site` refreshes the download block from the latest public release, and `./kaepora deploy` commits website changes, pushes them, and verifies the exact page is live. `./kaepora release [major|minor|patch|none]` builds, signs, notarizes, publishes the ZIP here, then updates and deploys the site. The updater reads this repository’s latest GitHub release.

## Usage statistics

This site records anonymous usage statistics: page views, download clicks and a daily visitor count derived from a hash of your IP address and browser. No cookies, no personal data, nothing stored in your browser. The collector is [Gossip Stone](https://github.com/iamjason/gossip-stone-swift#what-is-sent).
