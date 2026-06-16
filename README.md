# Giant US — Product Registration Prototype

A single-file front-end prototype recreating the [Giant Bicycles US product registration](https://www.giant-bicycles.com/us/registration) flow, with an integrated **Giant ID 3.0** sign-in / sign-up experience (modeled from Figma).

Pure HTML/CSS/JS — no backend, no build step. Works offline (assets and the Overpass font are self-hosted under `assets/`).

## Live preview

Served via GitHub Pages — see the repository's **Pages** URL.

## Flow

1. **Confirm Your Frame Number** — serial check disabled (any value proceeds); `E…` serials reveal an e-bike key field.
2. **Address & Contact info** — choose **Existing customer** (Giant ID login modal) or **New customer** (registration form). Filling a password + checking the consent box triggers an email **Verify code** modal; a successful sign-up shows a "Giant ID created" toast.
3. **Point of purchase** — authorized retailer search or "somewhere else".
4. **Purchase date**.
5. **Confirmation** — summary with the Giant ID account state.

A running summary panel (Your product / Contact info / Point of purchase) builds up on the right as steps complete.

## Notes

- Demo behaviors: any login is accepted; phone number `1111` simulates an "already registered" Giant ID on sign-up.
- Easter egg: **double-click any input** to auto-fill a sensible demo value.

Files: [`giant-us-registration-prototype.html`](giant-us-registration-prototype.html) is the prototype; `index.html` redirects to it for Pages.
