<h1 align="center">Ke Shen's Personal Website</h1>

<p align="center">Love, fate, the choices we make.</p>

<p align="center">
    <img src="assets/images/author.jpg" height="96" width="96" style="border-radius: 50%;">
</p>

<div align="center">

[![Cloudflare Pages](https://img.shields.io/badge/Deploy-Cloudflare%20Pages-f38020?style=flat&logo=cloudflare&logoColor=white)](https://keshen.link)
![GitHub repo size](https://img.shields.io/github/repo-size/shenke93/keshen.link)
![GitHub last commit](https://img.shields.io/github/last-commit/shenke93/keshen.link)

</div>

<div align="center">

✨ Live Preview: <https://keshen.link> ✨

</div>

---

This is the source code of my personal website and blog hosted at [keshen.link](https://keshen.link). Initially built in late 2024, it is a creative space for sharing technical insights, personal reflections, and creative writing. 

---

### 📦 Repository & Hosting

- **Primary Repository:** <https://github.com/shenke93/keshen.link>
- **Hosting Platform:** [Cloudflare Pages](https://pages.cloudflare.com/) (Global CDN Edge)

---

### 🎨 Theme & Submodules

This blog uses the [Blowfish](https://github.com/nunocoracao/blowfish) theme and integrates the [Mastodon Embed Timeline](https://github.com/eallion/mastodon-embed-timeline) library via Git submodules.

#### Clone & Initialize

```bash
# Clone recursively to fetch all submodules
git clone --recursive https://github.com/shenke93/keshen.link.git
cd keshen.link
```

If already cloned without submodules:
```bash
git submodule update --init --recursive
```

#### Update Submodules
```bash
git submodule update --remote --merge
```

---

### 🛠️ Working Commands

#### Local Development
Run the local Hugo development server:
```bash
hugo server -D
```

#### Build Production
Compile the site with minification:
```bash
hugo --minify
```

#### Cloudflare Pages Build Settings
If deploying automatically via Git integration:
- **Build command:** `hugo --minify`
- **Build output directory:** `public`
- **Environment variable:** `HUGO_VERSION` = `0.120.0` (or your preferred version)

If deploying manually via Wrangler:
```bash
npx wrangler pages deploy public
```

---

### ⚖️ License

- **Source Code:** [GLWT License](https://github.com/eallion/eallion.com/blob/main/LICENSE) (Good Luck With That License)
- **Content:** [Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/deed.zh)
