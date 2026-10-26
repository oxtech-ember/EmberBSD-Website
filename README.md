# EmberBSD Website

The public project page for [EmberBSD](https://github.com/oxtech-ember/EmberBSD).
Tagline: **Unix for creators and creatures**. EmberBSD is an independent
NetBSD 11 fork with a coherent base system and shared dependencies in Ports.
An AI agent can study the public sources and help adapt the system.

## Messaging

The homepage invites makers to imagine a device, follow the development path,
meet Spark, and start with a documented board and an application example. Three illustrated
project concepts show a workshop helper, a robot and a reused screen. They are
ideas, not photographs or demonstrations of accepted hardware.

Spark speaks in the first person in the notebook excerpt. His voice is curious,
dry and self-deprecating. He can dream about Mars while an old phone remains a prospect.
EmberBSD is his portable home. Use ordinary words for his digital belongings.
Keep the project voice factual. Do not present plans as completed experiments.
Published checks and their limits sit beside the plans, with links to the source.

The diary link is https://t.me/emberbsd_spark. Do not add a language label.
Add another social channel only after its real account is available.

The Unix and Ports sections explain shared interfaces and shared fixes.
The BSD history section links to primary sources. It does not imply affiliation,
endorsement, inherited hardware support or a security advantage over other systems.
State licenses by component. Do not describe the complete dependency tree as BSD-licensed.

The design follows the original flame mascot: warm paper, dark brown, burnt
orange and amber. Sora and the unchanged mascot are served locally. Inline SVG
concept sketches are original website illustrations. The page has no scripts.

Keep Spark optional. Mark phone, tablet, TV, creator-tool and general NPU work
as in development. Put board evidence in DevBoards and link to it. Do not claim
a speed or reliability advantage over Linux or complete hardware support.
The commercial edition is planned, not available. Do not publish private plans,
prices, budgets, team details or internal names. The site is English only.

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

## Search indexing

The homepage declares its canonical HTTPS URL. `docs/sitemap.xml` lists that page.
Keep both URLs in sync when connecting a custom domain. Keep the 404 page and
social-card source out of the sitemap; both have `noindex` metadata.

Add `https://oxtech-ember.github.io/EmberBSD-Website/` as a URL-prefix property in
[Google Search Console](https://search.google.com/search-console/).
Verify ownership with Google's HTML meta tag or verification file. Publish the
exact value supplied by the owner's account, then complete verification there.
Submit `https://oxtech-ember.github.io/EmberBSD-Website/sitemap.xml` and use URL
Inspection to check the homepage and request indexing. Keep the verification
tag or file after verification. Do not publish account credentials.

This project cannot serve the host-level `/robots.txt` from its `docs/` directory.
A file at `/EmberBSD-Website/robots.txt` would not control crawling.
The host currently returns 404 for `/robots.txt`, which does not block crawling.
See Google's [robots.txt rules](https://developers.google.com/crawling/docs/robots-txt/robots-txt-spec).

Indexing and search positions are not guaranteed. Use Search Console to check
the actual indexing status; a missing search result alone is not a diagnosis.

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
The [VM upgrade guide](https://github.com/oxtech-ember/EmberBSD/blob/main/doc/guide/amd64-vm-upgrade.md)
owns the procedure and its limits. This covers two builds of EmberBSD 1.0, not an
automatic rollback service or physical-device acceptance.

Check current public sources before updating support statements. Do not publish private
plans, internal addresses, personal logs, credentials or personalized images.
Write public content in English. Keep changes focused and explain validation limits.
The site was created and updated with assistance from OpenAI Codex.

Messaging on 25 October 2026 was checked against these public owners:

- [Spark scope](https://github.com/oxtech-ember/EmberBSD-Spark/blob/main/README.md)
  and [validation limits](https://github.com/oxtech-ember/EmberBSD-Spark/blob/main/docs/testing.md#validation-scope).
- [Ports shared dependencies](https://github.com/oxtech-ember/EmberBSD-Ports/blob/main/docs/update-ports.md#shared-base-dependencies).
- [EmberBSD additions license](https://github.com/oxtech-ember/EmberBSD/blob/main/ember/LICENSE)
  and [Spark license](https://github.com/oxtech-ember/EmberBSD-Spark/blob/main/LICENSE).
- The [DevBoards catalog](https://github.com/oxtech-ember/EmberBSD-DevBoards) and the published amd64 installation candidate.
- [NASA/TM—2006-214083](https://ntrs.nasa.gov/api/citations/20060008707/downloads/20060008707.pdf),
  section 6.1, printed page 11 (PDF page 17): the SAMS Interim Control Unit used NetBSD.
  The report's later SpreadRecorder prototype used Linux; do not merge those claims.
- [Netflix Open Connect](https://openconnect.netflix.com/en/appliances/): appliance software and FreeBSD contributions.
- [OpenSSH history](https://www.openssh.org/history.html): OpenBSD origins and the portable version.

The notebook is an introduction on this website, not evidence of phone installation
or a completed space project. The Telegram link opens the channel, not a specific post.

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

The 1200 × 630 social image is `docs/assets/social-card.png`.
Its source is `docs/assets/social-card.html`. It lays out the original mascot and bundled Sora font.
To refresh it, serve `docs/`, open that HTML at 1200 × 630 CSS pixels, and wait for the font and image.
Capture the page at device scale 1, without browser chrome or resizing, then inspect the PNG.
Keep its metadata dimensions in `docs/index.html` in sync. The source page has `noindex`.
The composition does not change the mascot's license.
