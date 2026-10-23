# EmberBSD Website

The public project page for [EmberBSD](https://github.com/oxtech-ember/EmberBSD).
Tagline: **Unix for creators and creatures**. EmberBSD is an independent
NetBSD 11 fork: one open system, from the kernel through Ports, that an AI
agent can study and adapt.

## Messaging

The homepage states that tagline, the single open tree, Spark as an optional
agent, and one OS family from microcontrollers to boards. Phones, tablets,
TVs, Plasma Mobile, Plasma Bigscreen, the commercial edition and the smart
home are marked in progress. Do not claim a speed or reliability advantage
over Linux. Do not list a device as supported without a
[DevBoards](https://github.com/oxtech-ember/EmberBSD-DevBoards) profile.
Do not publish private plans, prices, budgets, team details or internal names.
The site is English only.

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

The current download selects the immutable `c5d396f5698b68e956b29ee5b256bc7877e6c517`
installation candidate. Its amd64 UEFI no-X11 profile passed public GitHub HTTPS
installation and upgrade from the preceding build, followed by complete cold backup recovery.
The [VM upgrade guide](https://github.com/oxtech-ember/EmberBSD/blob/main/ember/boot/amd64-vm-upgrade.md)
owns the procedure and its limits. This covers two builds of EmberBSD 1.0, not an
automatic rollback service or physical-device acceptance.

Initial content was reviewed against:

- EmberBSD `7f5df9ed254d062f5fab03cc8f7a917b13df38e2`: README, build guide and board pages.
- EmberBSD-Ports `24fff6f2e0a58a48c3bfe0586ff5198cfabb9f43`: dependency profiles and source probes.
- Public EmberBSD-Examples application procedures.

Check current public sources before updating support statements. Do not publish private
plans, internal addresses, personal logs, credentials or personalized images.
Write public content in English. Keep changes focused and explain validation limits.
The site was created with assistance from OpenAI Codex GPT-6.

Messaging on 23 October 2026 was checked against the public OS guides,
the DevBoards catalog, Spark, the SDK, the KiCad, Plasma Mobile, Plasma
Bigscreen and smart-home Ports probes, and the published amd64 installation
candidate. Board links point at DevBoards. The former `ember/boards` paths
are not on the current OS tree. Guide links point at `doc/guide/`.

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
