---
sidebar_position: 1
slug: /setup
---

# Setup

## Cloning the CryoLayer Template Repository

The CryoLayer template repository is available on GitHub at [https://github.com/smarterlabs/cryolayer-worker](https://github.com/smarterlabs/cryolayer-worker).

Click the "Use this template" button, then click "Create a new repository". (See [GitHub's docs](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template#creating-a-repository-from-a-template) for more info if necessary.)

## Configuration Quickstart

Clone your new repository and install dependencies with `npm install` or `yarn`.

Edit the `config.js` file in the root of your repository. Make sure to set `webflowUrls` and `canonical` to the correct values.

For a full list of configuration options, see the [Configuration](/configuration) page.

## Deploying to Cloudflare Workers

### Install the Cloudflare CLI

The Cloudflare CLI is used to deploy your site to Cloudflare Workers. See [Cloudflare's docs](https://developers.cloudflare.com/workers/cli-wrangler/install-update) for installation instructions.

Run `wrangler login` and follow the instructions to log in to Cloudflare.

### Deploy your site

Run `wrangler deploy` to deploy your site to Cloudflare Workers. Your terminal will display a URL where your site is available.

Set your domain to point to your Cloudflare Workers site. See [Cloudflare's docs](https://developers.cloudflare.com/workers/platform/triggers/custom-domains/) for more info.