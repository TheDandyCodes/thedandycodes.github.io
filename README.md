# Ricardo Prieto Álvarez — Portfolio

A minimalist, highly functional portfolio website inspired by Swiss Typography (International Typographic Style) and Andrej Karpathy's text-based architecture. 

Designed for high contrast, strict grid alignment, and absolute clarity, prioritizing whitespace and clean typography.

## Design Philosophy

- **Typography**: Optimized stack prioritizing **Helvetica Neue** (macOS) and **Instrument Sans** (an open-source neo-grotesque alternative). Set with classic tight tracking (`letter-spacing: -0.035em` for headings, `-0.015em` for body).
- **Asymmetric Grid Layout**: Left-aligned dates, years, and headings in the left column (25% width), with content and flat visual cards aligned in the right column (75% width).
- **Tactile Hover Animations**: Minimalist micro-interactions including solid Swiss Red shadows on card hovers, rotating timeline diamond markers, and grayscale-to-color profile transitions.
- **ATS-Friendly Printing**: Print styles override grid properties, forcing a standard single-column text flow. Images, timeline paths, and stylized numbering prefixes are hidden, and LinkedIn/GitHub links dynamically print their destination URLs for optimal AI OCR parsing.

## How to View Locally

Open `index.html` directly in any modern browser, or run a local web server:

```bash
# Using Python / uv
uv run python -m http.server 8000
# or
python3 -m http.server 8000
```

Visit the site at `http://localhost:8000`.

## GitHub Pages Deployment

To publish this portfolio to your root domain (`https://thedandycodes.github.io/`):

### 1. Configure the GitHub Repository
1. Create a repository on GitHub named exactly: **`thedandycodes.github.io`**
2. In your local project directory, point your remote to this new name:
   ```bash
   git remote set-url origin https://github.com/TheDandyCodes/thedandycodes.github.io.git
   ```
3. Push your code to GitHub:
   ```bash
   git push -u origin main
   ```

### 2. Enable GitHub Pages
1. Go to repository **Settings** -> **Pages** on the web.
2. Under **Build and deployment** -> **Branch**, select **`main`** and **`/ (root)`**, then click **Save**.
3. *Note: If you get a "Deployment failed" status when renaming an existing repository, toggle the Branch setting to `None`, save, and then toggle it back to `main` and save again to force-clear GitHub's routing cache.*

## Custom Domain Setup

To link a custom domain (e.g. `ricardoprieto.com`):

1. In GitHub **Settings** -> **Pages**, enter your domain name under **Custom domain** and click **Save**.
2. Log in to your domain registrar (e.g. Porkbun, Namecheap) and add the following records:
   - **Main Domain (A Records)**: Add four `A` records pointing to GitHub's IPs:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - **WWW Subdomain (CNAME Record)**: Add a `CNAME` record with Host `www` pointing to `thedandycodes.github.io`.
3. In GitHub Settings, check **Enforce HTTPS** once the DNS propagates.

## How to Save as PDF

Click the **"Print Portfolio / Save as PDF"** link at the bottom of the page (hidden on print) or press `Cmd+P` / `Ctrl+P` in your browser. Select **Save as PDF** as the destination. Default browser headers and footers (like page numbers and date stamps) are automatically hidden in print mode.
