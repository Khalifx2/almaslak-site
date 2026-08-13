# Al-Maslak al-Muyassar — Site Files

Three pages, no build tools required:

- `index.html` — homepage
- `egypt-guide.html` — the full Egypt guide (visa, housing, institutes, budget calculator, checklist, FAQ, community)
- `housing-guide.html` — standalone housing guide

---

## 1. First-time deploy (10 minutes)

**Step 1 — Put the files on GitHub**
1. Go to [github.com](https://github.com) → sign in (or create a free account)
2. Click **New repository** → name it e.g. `almaslak-site` → set to **Public** → **Create repository**
3. On the new repo page, click **Add file → Upload files**
4. Drag in all three `.html` files (and this README) → **Commit changes**

**Step 2 — Connect Netlify**
1. Go to [netlify.com](https://netlify.com) → sign up **with your GitHub account** (this links them automatically)
2. Click **Add new site → Import an existing project → GitHub**
3. Select your `almaslak-site` repo
4. Leave all build settings blank/default (there's nothing to build — it's plain HTML) → **Deploy site**
5. Netlify gives you a live URL immediately (something like `almaslak-site.netlify.app`)

**Step 3 — Custom domain (optional, whenever you're ready)**
Buy a domain (Namecheap, ~£10/year) → in Netlify go to **Domain settings → Add custom domain** → follow their instructions to point your domain at Netlify.

From this point on, **any change you push to GitHub automatically redeploys the live site within ~30 seconds.** No re-uploading, no re-connecting anything.

---

## 2. Making quick text edits (after deploy)

For small changes — fixing a price, editing a sentence, updating a phone number — you don't need me or any tool installed. Do it straight on GitHub:

1. Go to your repo on github.com
2. Click the file you want to edit (e.g. `egypt-guide.html`)
3. Click the **pencil icon** (top right of the file view) — this opens GitHub's text editor
4. Use `Ctrl+F` / `Cmd+F` in your browser to find the text you want to change
5. Edit it directly
6. Scroll down → **Commit changes** (green button)
7. Netlify rebuilds automatically — check your live site in ~30 seconds

**This is genuinely just editing text between HTML tags** — you're not touching code logic, just the words. For example, to change a price you'd find something like:

```html
<span><strong>Cost:</strong> $200/level + ~$4 registration</span>
```

and just change `$200` to whatever the new price is, then commit.

### What's safe to edit yourself this way
- Prices, phone numbers, dates, addresses
- Any paragraph of text between `>` and `<`
- Links (the part inside `href="..."`)

### What NOT to touch (ask me instead)
- Anything inside `<script>` tags (JavaScript — the budget calculator, translate widget, path selector all live here)
- Anything inside `<style>` tags (CSS — layout and colours)
- The overall HTML structure (adding new cards/sections, not just editing existing text)

If you're ever unsure whether an edit is safe, paste me the before/after and I'll confirm — or just send me the change and I'll make it and tell you exactly what to paste in.

---

## 3. Bigger changes (new sections, redesigns, new institutes)

Come back here and ask — I'll make the edit to the file and give you the updated version to re-upload (drag-and-drop replace on GitHub, same as the first upload), or walk you through pasting a specific block of code into the GitHub editor.
