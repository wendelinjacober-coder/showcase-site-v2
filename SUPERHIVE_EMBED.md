# Superhive embed

Every product folder has a `superhive.html`: an interactive, dark card (big render, arrows, counter, category
chips, thumbnail strip, title, description, tags, controls). Keyboard arrows and swipe work too.

## 1. Renders

Put one **1920 × 1080 JPG per shader** into `<product>/img/1080/`.
The exact file names are listed in `<product>/img/1080/RENDER_LIST.txt`.
Until a file exists, the embed shows the old square preview, or a placeholder that names the missing file.
The Complete Library uses the renders of the single packs, nothing extra to render.

## 2. Host the folder

Upload the whole `showcase_site_v2` folder to any static host (your website, GitHub Pages, Netlify …),
so that for example `https://YOUR-SITE/stone-concrete-ceramic-shaders/superhive.html` opens in a browser.

## 3. Embed on the About page

```html
<iframe src="https://YOUR-SITE/stone-concrete-ceramic-shaders/superhive.html"
        style="width:100%;height:660px;border:0;border-radius:18px;overflow:hidden"
        loading="lazy" title="Stone, Concrete & Ceramic Shaders – shader browser"></iframe>
```

Height: about 660 px on desktop. The card stacks on narrow screens; if Superhive shows it narrow,
use `height:1000px`.

Folder names:

| Product | Folder |
|---|---|
| Complete Procedural Shader Library | complete-shader-library |
| Chrome Type Kit 2 | chrome-type-kit-2 |
| Abstract & Motion Graphics | abstract-motion-shaders |
| Automotive | automotive-shaders |
| Clay & Craft | clay-craft-shaders |
| Fabric & Fibre | fabric-fibre-shaders |
| Glass, Crystal & Liquid | glass-crystal-liquid-shaders |
| Ground | ground-shaders |
| Metal | metal-shaders |
| Organic & Creature | organic-creature-shaders |
| Paper & Cardboard | paper-cardboard-shaders |
| Plastic, Rubber & Foam | plastic-rubber-foam-shaders |
| Stone, Concrete & Ceramic | stone-concrete-ceramic-shaders |
| Stylized & NPR | stylized-npr-shaders |
| Weather: Ice, Snow & Rain | weather-ice-snow-rain-shaders |
| Wood | wood-shaders |

`embed.html` in each folder is the plain-HTML text version (no script) for places that do not allow iframes.
