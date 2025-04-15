<p align="center">
  <img src="/public/favicon.svg" width="50" alt="Logo" />
</p>
<h1 align="center">Personal portfolio</h1>

[![Site preview](/public/site-preview.png)](https://hamishw.com)

My design portfolio to showcase a few projects. Built with [Remix](https://remix.run/), [Three.js](https://threejs.org/), and [Framer Motion](https://www.framer.com/motion/). View the [live site](https://hamishw.com) or check out a live version of the [components storybook](https://storybook.hamishw.com).

## Install & run

Make sure you have nodejs `19.9.0` or higher and npm `9.6.3` or higher installed. Install dependencies with:

```bash
npm install
```

Once it's done start up a local server with:

```bash
npm run dev
```

To view the components storybook:

```bash
npm run dev:storybook
```

## Deployment

I've set up the site using Cloudflare for hosting. Deploy the site to Cloudflare Pages:

```bash
npm run deploy
```

## Permissions

I'm cool with anyone using the code or parts of the code for their own site, it is open source so people can learn from it and adapt it. However, I would encourage you to modify the theme and components it to make it your own. If you are using the site's design largely unmodified, I'd appreciate being credited as the designer of the website.

I do not give permission to present any of my projects as your own (this is being actively used as my portfolio site and these are my real projects I've worked on).

## FAQs

<details>
  <summary>How do I change the color on the <code>DisplacementSphere</code> (blobby rotating thing in the background).</summary>
  
  You'll need to edit the fragment shader. [Check out this issue for more details](https://github.com/HamishMW/portfolio/issues/19#issuecomment-870996615).
</details>

<details>
  <summary>How do I get the contact form to work?</summary>
  
  To get the contact form working create an AWS account and set up SES (Simple Email service). Then plug in your details into `.dev.vars.example` and rename it to `.dev.vars`. You'll also need to add these as enviroment variables in the Cloudflare dashboard for it to work in production. Or if you don't mind sending through gmail use [nodemailer](https://nodemailer.com/) instead.
</details>

```
portfolio-master
├─ .eslintrc.cjs
├─ .node-version
├─ .npmrc
├─ .prettierrc
├─ .storybook
│  ├─ main.js
│  ├─ manager-head.html
│  ├─ manager.js
│  ├─ preview.css
│  ├─ preview.jsx
│  ├─ story-container.css
│  ├─ story-container.jsx
│  └─ vite.config.js
├─ app
│  ├─ assets
│  │  ├─ earth.glb
│  │  ├─ flatline-alt.mp4
│  │  ├─ flatline.mp4
│  │  ├─ flatline.png
│  │  ├─ fonts
│  │  │  ├─ gotham-bold-italic.woff2
│  │  │  ├─ gotham-bold.woff2
│  │  │  ├─ gotham-book-italic.woff2
│  │  │  ├─ gotham-book.woff2
│  │  │  ├─ gotham-medium-italic.woff2
│  │  │  ├─ gotham-medium.woff2
│  │  │  └─ ipa-gothic.woff2
│  │  ├─ gamestack-list-large.jpg
│  │  ├─ gamestack-list-placeholder.jpg
│  │  ├─ gamestack-list.jpg
│  │  ├─ gamestack-login-large.jpg
│  │  ├─ gamestack-login-placeholder.jpg
│  │  ├─ gamestack-login.jpg
│  │  ├─ iphone-11.glb
│  │  ├─ macbook-pro.glb
│  │  ├─ milkyway-nx.hdr
│  │  ├─ milkyway-ny.hdr
│  │  ├─ milkyway-nz.hdr
│  │  ├─ milkyway-px.hdr
│  │  ├─ milkyway-py.hdr
│  │  ├─ milkyway-pz.hdr
│  │  ├─ milkyway.hdr
│  │  ├─ milkyway.jpg
│  │  ├─ notfound.jpg
│  │  ├─ notfound.mp4
│  │  ├─ profile-large.jpg
│  │  ├─ profile-placeholder.jpg
│  │  ├─ profile.jpg
│  │  ├─ slice-annotation-large.png
│  │  ├─ slice-annotation-placeholder.png
│  │  ├─ slice-annotation.png
│  │  ├─ slice-app-large.jpg
│  │  ├─ slice-app-placeholder.jpg
│  │  ├─ slice-app.jpg
│  │  ├─ slice-background-bar-large.jpg
│  │  ├─ slice-background-bar-placeholder.jpg
│  │  ├─ slice-background-bar.jpg
│  │  ├─ slice-background-large.jpg
│  │  ├─ slice-background-placeholder.jpg
│  │  ├─ slice-background.jpg
│  │  ├─ slice-irl-placeholder.jpg
│  │  ├─ slice-irl.jpg
│  │  ├─ slice-sidebar-annotations-large.png
│  │  ├─ slice-sidebar-annotations-placeholder.png
│  │  ├─ slice-sidebar-annotations.png
│  │  ├─ slice-sidebar-layers-large.png
│  │  ├─ slice-sidebar-layers-placeholder.png
│  │  ├─ slice-sidebar-layers.png
│  │  ├─ slice-slides-large.jpg
│  │  ├─ slice-slides-placeholder.jpg
│  │  ├─ slice-slides.jpg
│  │  ├─ spr-background-large.jpg
│  │  ├─ spr-background-placeholder.jpg
│  │  ├─ spr-background-volcanism-large.jpg
│  │  ├─ spr-background-volcanism-placeholder.jpg
│  │  ├─ spr-background-volcanism.jpg
│  │  ├─ spr-background.jpg
│  │  ├─ spr-components-dark-large.png
│  │  ├─ spr-components-dark-placeholder.png
│  │  ├─ spr-components-dark.png
│  │  ├─ spr-components-light-large.png
│  │  ├─ spr-components-light-placeholder.png
│  │  ├─ spr-components-light.png
│  │  ├─ spr-design-system-dark-large.png
│  │  ├─ spr-design-system-dark-placeholder.png
│  │  ├─ spr-design-system-dark.png
│  │  ├─ spr-design-system-light-large.png
│  │  ├─ spr-design-system-light-placeholder.png
│  │  ├─ spr-design-system-light.png
│  │  ├─ spr-lesson-builder-dark-large.jpg
│  │  ├─ spr-lesson-builder-dark-placeholder.jpg
│  │  ├─ spr-lesson-builder-dark.jpg
│  │  ├─ spr-lesson-builder-light-large.jpg
│  │  ├─ spr-lesson-builder-light-placeholder.jpg
│  │  ├─ spr-lesson-builder-light.jpg
│  │  ├─ spr-motion-large.mp4
│  │  ├─ spr-motion-placeholder.jpg
│  │  ├─ spr-motion.mp4
│  │  ├─ spr-schema-1-dark-large.png
│  │  ├─ spr-schema-1-dark-placeholder.png
│  │  ├─ spr-schema-1-dark.png
│  │  ├─ spr-schema-1-light-large.png
│  │  ├─ spr-schema-1-light-placeholder.png
│  │  ├─ spr-schema-1-light.png
│  │  ├─ spr-schema-2-dark-large.png
│  │  ├─ spr-schema-2-dark-placeholder.png
│  │  ├─ spr-schema-2-dark.png
│  │  ├─ spr-schema-2-light-large.png
│  │  ├─ spr-schema-2-light-placeholder.png
│  │  ├─ spr-schema-2-light.png
│  │  ├─ spr-storyboarder-dark-large.png
│  │  ├─ spr-storyboarder-dark-placeholder.png
│  │  ├─ spr-storyboarder-dark.png
│  │  ├─ spr-storyboarder-light-large.png
│  │  ├─ spr-storyboarder-light-placeholder.png
│  │  ├─ spr-storyboarder-light.png
│  │  ├─ uses-background-placeholder.jpg
│  │  ├─ uses-background.mp4
│  │  ├─ volkihar-background-large.jpg
│  │  ├─ volkihar-background-placeholder.jpg
│  │  ├─ volkihar-background.jpg
│  │  ├─ volkihar-banner-large.jpg
│  │  ├─ volkihar-banner-placeholder.jpg
│  │  ├─ volkihar-banner.jpg
│  │  ├─ volkihar-book-large.png
│  │  ├─ volkihar-book-placeholder.png
│  │  ├─ volkihar-book.png
│  │  ├─ volkihar-cube-nx.jpg
│  │  ├─ volkihar-cube-ny.jpg
│  │  ├─ volkihar-cube-nz.jpg
│  │  ├─ volkihar-cube-px.jpg
│  │  ├─ volkihar-cube-py.jpg
│  │  ├─ volkihar-cube-pz.jpg
│  │  ├─ volkihar-enderal-large.jpg
│  │  ├─ volkihar-enderal-logo-large.png
│  │  ├─ volkihar-enderal-logo-placeholder.png
│  │  ├─ volkihar-enderal-logo.png
│  │  ├─ volkihar-enderal-placeholder.jpg
│  │  ├─ volkihar-enderal.jpg
│  │  ├─ volkihar-knight.glb
│  │  ├─ volkihar-slide-1-large.jpg
│  │  ├─ volkihar-slide-1.jpg
│  │  ├─ volkihar-slide-2-large.jpg
│  │  ├─ volkihar-slide-2.jpg
│  │  ├─ volkihar-slide-3-large.jpg
│  │  ├─ volkihar-slide-3.jpg
│  │  └─ volkihar-slide-placeholder.jpg
│  ├─ components
│  │  ├─ button
│  │  │  ├─ button.jsx
│  │  │  ├─ button.module.css
│  │  │  ├─ button.stories.jsx
│  │  │  └─ index.js
│  │  ├─ carousel
│  │  │  ├─ carousel-fragment.glsl
│  │  │  ├─ carousel-vertex.glsl
│  │  │  ├─ carousel.jsx
│  │  │  ├─ carousel.module.css
│  │  │  ├─ carousel.stories.jsx
│  │  │  └─ index.js
│  │  ├─ code
│  │  │  ├─ code.jsx
│  │  │  ├─ code.module.css
│  │  │  └─ index.js
│  │  ├─ decoder-text
│  │  │  ├─ decoder-text.jsx
│  │  │  ├─ decoder-text.module.css
│  │  │  ├─ decoder-text.stories.jsx
│  │  │  └─ index.js
│  │  ├─ divider
│  │  │  ├─ divider.jsx
│  │  │  ├─ divider.module.css
│  │  │  └─ index.js
│  │  ├─ footer
│  │  │  ├─ footer.jsx
│  │  │  ├─ footer.module.css
│  │  │  └─ index.js
│  │  ├─ heading
│  │  │  ├─ heading.jsx
│  │  │  ├─ heading.module.css
│  │  │  ├─ heading.stories.jsx
│  │  │  └─ index.js
│  │  ├─ icon
│  │  │  ├─ icon.jsx
│  │  │  ├─ icon.module.css
│  │  │  ├─ icon.stories.jsx
│  │  │  ├─ icons.svg
│  │  │  ├─ index.js
│  │  │  └─ manifest.json
│  │  ├─ image
│  │  │  ├─ image.jsx
│  │  │  ├─ image.module.css
│  │  │  ├─ image.stories.jsx
│  │  │  └─ index.js
│  │  ├─ input
│  │  │  ├─ index.js
│  │  │  ├─ input.jsx
│  │  │  ├─ input.module.css
│  │  │  ├─ input.stories.jsx
│  │  │  ├─ text-area.jsx
│  │  │  └─ text-area.module.css
│  │  ├─ link
│  │  │  ├─ index.js
│  │  │  ├─ link.jsx
│  │  │  ├─ link.module.css
│  │  │  └─ link.stories.jsx
│  │  ├─ list
│  │  │  ├─ index.js
│  │  │  ├─ list.jsx
│  │  │  ├─ list.module.css
│  │  │  └─ list.stories.jsx
│  │  ├─ loader
│  │  │  ├─ index.js
│  │  │  ├─ loader.jsx
│  │  │  ├─ loader.module.css
│  │  │  └─ loader.stories.jsx
│  │  ├─ model
│  │  │  ├─ device-models.js
│  │  │  ├─ index.js
│  │  │  ├─ model.jsx
│  │  │  ├─ model.module.css
│  │  │  └─ model.stories.jsx
│  │  ├─ monogram
│  │  │  ├─ index.js
│  │  │  ├─ monogram.jsx
│  │  │  ├─ monogram.module.css
│  │  │  └─ Monogram.stories.jsx
│  │  ├─ progress
│  │  │  ├─ index.js
│  │  │  ├─ progress.jsx
│  │  │  └─ progress.module.css
│  │  ├─ section
│  │  │  ├─ index.js
│  │  │  ├─ section.jsx
│  │  │  └─ section.module.css
│  │  ├─ segmented-control
│  │  │  ├─ index.js
│  │  │  ├─ segmented-control.jsx
│  │  │  ├─ segmented-control.module.css
│  │  │  └─ segmented-control.stories.jsx
│  │  ├─ table
│  │  │  ├─ index.js
│  │  │  ├─ table.jsx
│  │  │  ├─ table.module.css
│  │  │  └─ table.stories.jsx
│  │  ├─ text
│  │  │  ├─ index.js
│  │  │  ├─ text.jsx
│  │  │  ├─ text.module.css
│  │  │  └─ text.stories.jsx
│  │  ├─ theme-provider
│  │  │  ├─ index.js
│  │  │  ├─ theme-provider.jsx
│  │  │  └─ theme.js
│  │  ├─ transition
│  │  │  ├─ index.js
│  │  │  └─ transition.jsx
│  │  └─ visually-hidden
│  │     ├─ index.js
│  │     ├─ visually-hidden.jsx
│  │     └─ visually-hidden.module.css
│  ├─ config.json
│  ├─ global.module.css
│  ├─ hooks
│  │  ├─ index.js
│  │  ├─ useFormInput.js
│  │  ├─ useHasMounted.js
│  │  ├─ useHydrated.js
│  │  ├─ useInterval.js
│  │  ├─ useInViewport.js
│  │  ├─ useParallax.js
│  │  ├─ usePrevious.js
│  │  ├─ useScrollToHash.js
│  │  └─ useWindowSize.js
│  ├─ layouts
│  │  ├─ error
│  │  │  ├─ error-flatline.svg
│  │  │  ├─ error.jsx
│  │  │  ├─ error.module.css
│  │  │  └─ index.js
│  │  ├─ navbar
│  │  │  ├─ index.js
│  │  │  ├─ nav-data.js
│  │  │  ├─ nav-toggle.jsx
│  │  │  ├─ nav-toggle.module.css
│  │  │  ├─ navbar.jsx
│  │  │  ├─ navbar.module.css
│  │  │  ├─ theme-toggle.jsx
│  │  │  └─ theme-toggle.module.css
│  │  ├─ post
│  │  │  ├─ index.js
│  │  │  ├─ post-markdown.jsx
│  │  │  ├─ post-markdown.module.css
│  │  │  ├─ post.jsx
│  │  │  └─ post.module.css
│  │  └─ project
│  │     ├─ index.js
│  │     ├─ project.jsx
│  │     └─ project.module.css
│  ├─ reset.module.css
│  ├─ root.jsx
│  ├─ root.module.css
│  ├─ routes
│  │  ├─ $.jsx
│  │  ├─ api.set-theme.js
│  │  ├─ articles
│  │  │  └─ route.jsx
│  │  ├─ articles.hello-world.mdx
│  │  ├─ articles.modern-styling-in-react.mdx
│  │  ├─ articles_._index
│  │  │  ├─ articles.jsx
│  │  │  ├─ articles.module.css
│  │  │  ├─ posts.server.js
│  │  │  └─ route.jsx
│  │  ├─ contact
│  │  │  ├─ contact.jsx
│  │  │  ├─ contact.module.css
│  │  │  └─ route.js
│  │  ├─ home
│  │  │  ├─ displacement-sphere-fragment.glsl
│  │  │  ├─ displacement-sphere-vertex.glsl
│  │  │  ├─ displacement-sphere.jsx
│  │  │  ├─ displacement-sphere.module.css
│  │  │  ├─ home.jsx
│  │  │  ├─ home.module.css
│  │  │  ├─ intro.jsx
│  │  │  ├─ intro.module.css
│  │  │  ├─ katakana.svg
│  │  │  ├─ profile.jsx
│  │  │  ├─ profile.module.css
│  │  │  ├─ project-summary.jsx
│  │  │  ├─ project-summary.module.css
│  │  │  └─ route.js
│  │  ├─ projects.slice
│  │  │  ├─ route.js
│  │  │  ├─ slice.jsx
│  │  │  └─ slice.module.css
│  │  ├─ projects.smart-sparrow
│  │  │  ├─ earth.jsx
│  │  │  ├─ earth.module.css
│  │  │  ├─ route.js
│  │  │  ├─ smart-sparrow.jsx
│  │  │  └─ smart-sparrow.module.css
│  │  ├─ projects.volkihar-knight
│  │  │  ├─ armor.jsx
│  │  │  ├─ armor.module.css
│  │  │  ├─ route.js
│  │  │  ├─ volkihar-knight.jsx
│  │  │  ├─ volkihar-knight.module.css
│  │  │  └─ volkihar-logo.jsx
│  │  └─ uses
│  │     ├─ route.js
│  │     ├─ uses.jsx
│  │     └─ uses.module.css
│  └─ utils
│     ├─ clamp.js
│     ├─ date.js
│     ├─ delay.js
│     ├─ image.js
│     ├─ mdx.js
│     ├─ meta.js
│     ├─ style.js
│     ├─ three.js
│     ├─ throttle.js
│     └─ timecode.js
├─ functions
│  └─ [[path]].js
├─ jsconfig.json
├─ LICENSE
├─ package-lock.json
├─ package.json
├─ postcss.config.cjs
├─ public
│  ├─ favicon.ico
│  ├─ favicon.svg
│  ├─ humans.txt
│  ├─ icon-256.png
│  ├─ icon-512.png
│  ├─ icon.svg
│  ├─ manifest.json
│  ├─ robots.txt
│  ├─ shortcut.png
│  ├─ site-preview.png
│  ├─ sitemap.xml
│  ├─ social-image.png
│  ├─ static
│  │  ├─ avatar.jpg
│  │  ├─ clay-mockups.png
│  │  ├─ hello-world-banner-placeholder.jpg
│  │  ├─ hello-world-banner.jpg
│  │  ├─ hello-world-og.jpg
│  │  ├─ inspiration.png
│  │  ├─ modern-styling-in-react-banner-placeholder.jpg
│  │  ├─ modern-styling-in-react-banner.jpg
│  │  ├─ modern-styling-in-react-og.jpg
│  │  └─ og-blank.png
│  └─ _headers
├─ README.md
├─ scripts
│  ├─ dev.cjs
│  └─ draco.cjs
├─ vite.config.js
└─ wrangler.toml

```