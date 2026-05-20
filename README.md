# sotoia · links

A personal link-in-bio page with the Liquid Gradient as background. One HTML file. Zero dependencies. Deploys anywhere static.

## Edit your profile

Open `index.html` and find the `PROFILE` and `LINKS` blocks near the bottom of the `<script>` tag:

```js
const PROFILE = {
  name: 'sotoia',
  handle: '@sotoia · developer · founder',
  bio: 'Building tools at the intersection of design and AI.',
  avatar: 'S',  // single letter, OR a URL: 'https://example.com/me.jpg'
};

const LINKS = [
  { label: 'YouTube', handle: '@sotoia', url: 'https://youtube.com/@sotoia', icon: 'youtube' },
  // ...add as many as you want
];
```

Available icons: `youtube`, `instagram`, `tiktok`, `x`, `github`, `linkedin`, `threads`, `sparkles`, `link`, `mail`, `globe`, `music`. Add new ones in the `ICONS` object.

## Deploy — free

### Option A · Vercel (recommended)

```sh
# from this folder
git init && git add . && git commit -m "init"
# push to a new repo on github.com/new, then:
# vercel.com → Add New Project → import repo → Deploy
```

You get `<project-name>.vercel.app` for free. Auto-redeploys on every push.

### Option B · GitHub Pages

```sh
# push to github.com/<username>/<repo>
# Repo Settings → Pages → Source: main / root → Save
# Wait 2 minutes
```

You get `<username>.github.io/<repo>` for free.

### Option C · Cloudflare Pages

Push to GitHub → cloudflare.com → Pages → Connect to GitHub → pick repo → Deploy. You get `<project>.pages.dev` for free.

## Custom domain (~$10-15/year)

For a personal link-in-bio, the slick TLDs are:

| TLD | ~Price/year | Why |
|-----|------------|-----|
| `.link` | $10-15 | Literally what this is |
| `.bio` | $10-15 | Same vibe |
| `.me` | $10-15 | Classic personal |
| `.so` | $8-15 | Short and modern |
| `.fyi` | $10-15 | Casual |

Buy on **Namecheap** or **Cloudflare Registrar** (Cloudflare is cheaper, no markup). Once you have it:

- Vercel: Project Settings → Domains → Add → `sotoia.link` → copy CNAME → add to DNS → done in 5 min
- Cloudflare Pages: similar flow inside Cloudflare dashboard

## Credits

Built with [Liquid Gradient](https://github.com/sotoia/liquid-gradient). MIT.
