# EmberBSD Website

The public project page for [EmberBSD](https://github.com/oxtech-ember/EmberBSD),
an independent NetBSD 11 fork for intelligent devices.

Site: **https://oxtech-ember.github.io/EmberBSD-Website/**

## Publish

The site is static HTML and CSS, with no JavaScript, package dependencies or build step.
GitHub Pages publishes `docs/` from `main`. `docs/.nojekyll` disables Jekyll processing.
Changes to that source branch trigger the GitHub-managed Pages deployment.
Keep the repository public. A custom domain is not configured yet.

Preview `docs/` with a local static HTTP server. The page uses relative asset paths
so it works below the GitHub project path. The custom 404 page uses that project
path explicitly; update it when connecting a custom domain.

Before publishing, check desktop and phone widths, keyboard navigation, contrast,
internal anchors, all asset responses and the linked public source documents.
Check the deployed commit, Pages build, HTTP response and rendered page after publishing.

## Content and boundaries

The site introduces the OS, optional application stacks, board support and ways to start.
Each claim links to its owning public repository. Board pages own hardware evidence;
the website is an introduction, not a replacement for build or installation instructions.
Keep source/build/VM/hardware results distinct. General installation images, a working
NPU backend, SDK/Runtime implementations and untested board support are not implied.
Download images and OS sets belong to the separate release channel, not this repository.

Initial content was reviewed against:

- EmberBSD `7f5df9ed254d062f5fab03cc8f7a917b13df38e2`: README, build guide and board pages.
- EmberBSD-Ports `24fff6f2e0a58a48c3bfe0586ff5198cfabb9f43`: dependency profiles and source probes.
- Public EmberBSD-Examples application procedures.

Check current public sources before updating support statements. Do not publish private
plans, internal addresses, personal logs, credentials or personalized images.
Write public content in English. Keep changes focused and explain validation limits.
The site was created with assistance from OpenAI Codex GPT-6.

## Assets and licensing

The flame mascot is copied unchanged from
[EmberBSD's public branding asset](https://github.com/oxtech-ember/EmberBSD/blob/7f5df9ed254d062f5fab03cc8f7a917b13df38e2/ember/branding/emberbsd-logo.png).
Its original source path is `ember/branding/emberbsd-logo.png`.
The mascot remains the EmberBSD project's branding asset. Preserve its identity and provenance;
the website code license does not relicense the original mascot.

Sora is bundled from [Google Fonts](https://github.com/google/fonts/tree/66928797f271fed5ee428544e7229685e2d90127/ofl/sora).
Its original filename is `Sora[wght].ttf`; the local filename is `sora.ttf`.
Font SHA256: `84ff7096ae3ec6c8be47d906d1a0ba4de7f2ce78c615275c77301964a316e16c`.
Mascot SHA256: `f4c6439f9c3da954fab7d5d3f2e16d46bb76c26431e0244a405dc4bf1ed992d6`.
Keep the original SIL OFL notice beside the font. Fonts and imagery are served locally;
the site does not make third-party font requests or include tracking scripts.

Website code uses [BSD-2-Clause](LICENSE). Upstream OS and companion components retain
their own authorship and licenses.
