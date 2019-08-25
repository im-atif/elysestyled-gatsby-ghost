# elysestyled.com

> Gatsby front-end for elysestyled.com, using Ghost as a headless CMS.

[![Netlify Status](https://api.netlify.com/api/v1/badges/115a4c63-abc2-42f3-9455-828b61e58967/deploy-status)](https://app.netlify.com/sites/elyse-styled-gatsby/deploys)

## Architecture

This site works by:

* a DigitalOcean droplet runs Ghost as a headless CMS
* posts are written on Ghost CMS
* this repo, for the Gatsby front-end and Ghost theme, based off [gatsby-starter-ghost](https://github.com/TryGhost/gatsby-starter-ghost).
* Netlify deploys this repo as a static site with `gatsby build` whenever the `elyse-theme` branch is updated
* TODO: Ghost is [integrated with Netlify](https://ghost.org/integrations/netlify/) to run whenever there is new content

## Local Installation

To edit this theme/front-end, download the repo and run `yarn` to install or update. Then start the development server. 

```bash
gatsby develop
```

This pulls content from `elysestyled.com` with settings in `.ghost.json`.

*TODO* add how to steps on running/building CSS, other tools, etc.

## Netlify Deploy

Any push update to the `elyse-theme` branch should automatically update Netlify at https://elyse-styled-gatsby.netlify.com/

