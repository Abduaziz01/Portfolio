# Dev Portfolio Template

> One HTML file. No frameworks. No build tools.

---

## Quick Start

Download `index.html` and open it in your browser. Done.

---

## Customization Guide

### 1. Name and Title

Find around line 60:

```html
<span class="fn">Abduaziz</span>
<span class="ln">Rustamov</span>
<div class="eyebrow">Full-Stack Developer</div>
```

### 2. Bio and Stats

```html
<p class="bio">
  <b>16 y.o.</b> full-stack dev from Uzbekistan.
</p>
```

Stats (find in the script block):

```js
cnt('ca', 16)       // age
cnt('cp', 12, '+')  // projects
cnt('ct', 15, '+')  // techs
```

### 3. Social Links

Find and replace these 3 values everywhere (Ctrl+H):

| Find | Replace |
|---|---|
| `abduaziz01` | your GitHub username |
| `agentxesil` | your Telegram username |
| `abduazizbuba@gmail.com` | your email |

### 4. Typewriter Words

```js
const words = [
  'Full-Stack Dev',
  'Backend Engineer',
  'Frontend Builder',
  'Open to Work',
  'Script Automator',
];
```

### 5. About Section

```html
<p class="at"><b>Your Name</b> - born <b>Month DD, YYYY</b>.</p>
<p class="at">What you build. 1-2 sentences.</p>

<!-- chips -->
<span class="ch">Your Skill</span>
```

Code card:

```html
<span class="v">"Your Name"</span>
<span class="vb">XX</span>        <!-- age -->
<span class="v">"YYYY-MM-DD"</span>
<span class="v">"Your Country"</span>
<span class="v">"yourusername"</span>
```

### 6. Skill Bars

```html
<div class="si">
  <div class="st2">
    <span class="sna">Skill Name</span>
    <span class="sp">85%</span>
  </div>
  <div class="sb">
    <div class="sf g" data-w="85"></div>  <!-- g=green, b=blue -->
  </div>
</div>
```

### 7. Projects

```html
<div class="pc rv">
  <div class="pi" style="background:linear-gradient(135deg,#030e18,#051a10)">
    emoji
  </div>
  <div class="pib">
    <div class="pbs">
      <span class="pbg n">Tech</span>     <!-- n=green -->
      <span class="pbg bl">Tech</span>    <!-- bl=blue -->
      <span class="pbg pu">Tech</span>    <!-- pu=purple -->
    </div>
    <div class="pt">Project Title</div>
    <div class="pd">Short description.</div>
    <div class="pls">
      <a class="pl" href="YOUR_GITHUB_REPO" target="_blank">GitHub</a>
      <a class="pl" href="YOUR_LIVE_LINK" target="_blank">Live</a>
    </div>
  </div>
</div>
```

Card background options:

```
Dark blue:   linear-gradient(135deg,#030e18,#040d20)
Purple:      linear-gradient(135deg,#060518,#100525)
Dark green:  linear-gradient(135deg,#040f04,#081a08)
Dark teal:   linear-gradient(135deg,#000e10,#001a1a)
Dark red:    linear-gradient(135deg,#180303,#200a04)
```

### 8. Colors

All in `:root` at the top:

```css
:root {
  --neon:   #00ffc8;  /* main accent  */
  --blue:   #4090ff;  /* secondary    */
  --purple: #a060ff;  /* tertiary     */
  --bg:     #030810;  /* background   */
}
```

After changing `--neon`, update the 3D crystal too:

```js
emissive: 0x00ffc8,  // match your --neon (no #)
color:    0x00ffc8,  // wireframe
```

Color presets:

| Theme | --neon | --blue |
|---|---|---|
| Orange | #ff6040 | #ff9020 |
| Purple | #c060ff | #6090ff |
| Gold | #ffd700 | #ffaa00 |
| Pink | #ff40a0 | #a040ff |

---

## What's Inside

| Feature | How |
|---|---|
| 3D crystal + rings + satellites | Three.js ES Module |
| DNA helix background | Canvas 2D |
| Glitch name effect | CSS keyframes |
| Neon cursor trail | Vanilla JS |
| Typewriter | Vanilla JS |
| Scroll reveal | IntersectionObserver |
| Floating code snippets | DOM + CSS animation |

---

## Deploy Free

**GitHub Pages:**
1. Create repo, upload file as `index.html`
2. Settings -> Pages -> Deploy from main
3. Live at `yourusername.github.io/repo`

**Netlify Drop (easiest):**
1. Go to app.netlify.com/drop
2. Drag the file
3. Instant URL

---

## License

Free to use and modify. Credit appreciated.

*Template by [Abduaziz Rustamov](https://github.com/abduaziz01) - [@agentxesil](https://t.me/agentxesil)*
