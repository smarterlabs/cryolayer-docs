---
sidebar_position: 4
slug: /updating
---

# Updating CryoLayer

To update your site with the latest CryoLayer template repository changes, follow these steps in [Git](https://git-scm.com/):

1. Open a terminal and navigate to your CryoLayer repository
2. Run `git remote add git@github.com:smarterlabs/cryolayer-proxy.git cryolayer`
3. Run `git fetch cryolayer`
4. Run `git merge cryolayer/main`
5. Resolve any merge conflicts
6. Run `git push origin main`
7. Run `wrangler publish` to deploy your site to Cloudflare Workers