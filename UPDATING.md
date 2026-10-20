# Updating the site

## Quick edit (in the browser)

1. On GitHub, open `index.html` and click the pencil icon.
2. Make your changes, then click **Commit changes**.
3. Pages republishes on its own in about a minute. If you don't see the change, hard-refresh (Cmd/Ctrl+Shift+R).

## Edit on your computer

```bash
git clone https://github.com/jb-db05/AI-rings-PublicVersion.git
cd AI-rings-PublicVersion
# open index.html in a browser to preview, edit it in any text editor
git add index.html
git commit -m "Update data"
git push
```

## Where things live in index.html

- **Title and intro text**: the `<header>` block near the top.
- **Styles and colours**: the `<style>` block in `<head>`.
- **Nodes, deals, funding stress**: the data objects in the `<script>` at the bottom (`N` = nodes, `D` = deals, `PR` = funding stress). Deals still carry a `src` field, but sources are no longer shown on the page.
- **Logo**: the `<img src="data:image/png;base64,...">` in the header. To swap it, add `logo.png` to the repo and change the tag to `src="logo.png"`.

## Check before you push

- Open `index.html` in a browser and click through a few nodes.
- Open the browser console (F12) and make sure there are no red errors.
