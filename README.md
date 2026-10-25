# H&H Contracting website

A simple one-page website for H&H Contracting, ready to host for free on GitHub Pages.

## Files

| File | What it is |
|---|---|
| `index.html` | The page content: text, sections, contact form |
| `styles.css` | The look: colors, fonts, layout |
| `images/logo.svg` | The logo |
| `images/deck.jpg` | The photo in the top section |

## Put it online with GitHub Pages

1. Create a free account at github.com and make a new **public** repository (for example `hh-contracting`).
2. Click **Add file → Upload files**, drag in everything from this folder (keep the `images` folder), and click **Commit changes**.
3. Go to **Settings → Pages**. Under "Build and deployment", set **Source** to *Deploy from a branch*, choose the `main` branch and the `/ (root)` folder, and click **Save**.
4. After a minute or two the site is live at `https://YOUR-USERNAME.github.io/hh-contracting/`.

To use your own domain (like `hhcontracting.com`), buy it from any registrar, then enter it under **Settings → Pages → Custom domain** and follow GitHub's DNS instructions.

## Fill in the placeholders

Search `index.html` for square brackets and replace each one with real details:
`[PHONE NUMBER]`, `[EMAIL]`, `[SERVICE AREA]`, `[OWNER NAME]`, `[NUMBER]` (license), and the about paragraph.
Also update the phone link: change `tel:+10000000000` to the real number, like `tel:+18015551234`.

## Change the color scheme

All colors live at the top of `styles.css`, in the `:root { ... }` block. Change the hex codes and the whole site updates.
The logo has its own two colors, so also open `images/logo.svg` and change the roof color (`#D9541E`) and the H color (`#FFFFFF`) to match.

Other schemes from the design board:

| Variable | Charcoal & Safety Orange (current) | Navy & Copper | Timber & Amber | Blueprint & Brick |
|---|---|---|---|---|
| `--primary` | `#26282B` | `#1E2B34` | `#23362B` | `#142A45` |
| `--accent` | `#D9541E` | `#A84A22` | `#C27E12` | `#CF3F2E` |
| `--accent-text` | `#B23F10` | `#A84A22` | `#8A5A0C` | `#B33526` |
| `--button-text` | `#14130F` | `#FFFFFF` | `#14130F` | `#FFFFFF` |
| `--background` | `#F2F2EF` | `#F4F0E8` | `#EFEBDF` | `#F4F6F8` |
| `--warm` | `#C8A27A` | `#D8C7A3` | `#C9B48A` | `#D9CFBF` |
| `--body-text` | `#43464A` | `#3D4950` | `#3F4A42` | `#3A4656` |
| `--muted-text` | `#5C6166` | `#5E666A` | `#5B655D` | `#5A6472` |
| `--border` | `#D9D9D4` | `#D8D2C6` | `#D6D0BF` | `#D3D9E0` |
| `--input-border` | `#7D8287` | `#8C9396` | `#7A8076` | `#7D8896` |
| `--on-dark` | `#F2F2EF` | `#F4F0E8` | `#EFEBDF` | `#F4F6F8` |
| `--on-dark-muted` | `#C9CCCF` | `#C9CDCF` | `#C8CEC5` | `#C3CCD6` |

## Change the logo

Replace `images/logo.svg` with a new file of the **same name**. It appears in the header and as the browser-tab icon.

## Change the photo

Replace `images/deck.jpg` with a photo of a finished job (same name), or update the `src` in `index.html`. A landscape photo around 1600 pixels wide works best.

## Make the contact form work

GitHub Pages can't receive form submissions by itself, so the form uses Formspree (free tier available):

1. Sign up at formspree.io and create a new form with the email address that should get requests.
2. Copy the form ID (the part after `/f/` in the endpoint it gives you).
3. In `index.html`, replace `YOUR_FORM_ID` in the form's `action` with that ID.
