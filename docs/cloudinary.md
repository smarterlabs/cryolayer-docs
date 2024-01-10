---
sidebar_position: 2
slug: /cloudinary
---

# Cloudinary Integration

CryoLayer integrates with [Cloudinary](https://cloudinary.com/) to provide image optimization and automatic WebP conversion.

## Setup

Create a Cloudinary account at [https://cloudinary.com/users/register/free](https://cloudinary.com/users/register/free).

Copy your cloud name from the dashboard. Paste it into the `cloudinaryCloudName` property in `config.js`.

## Image CDN Mapping

Now we'll set up the image mapping your Cloudinary account knows what which Webflow image domains to proxy.

Go to your Cloudinary account settings page and click the "Upload" menu link on the left.

Make sure "Auto-create folders" is enabled.

Click the "Add folder mapping" button.

Enter the following values:

Folder | URL prefix
--- | ---
`cryolayer/a` | `https://assets.website-files.com/`
`cryolayer/b` | `https://assets-global.website-files.com/`
`cryolayer/c` | `https://uploads-ssl.webflow.com/`
`cryolayer/d` | `https://global-uploads.webflow.com/`
`cryolayer/e` | `https://d3e54v103j8qbb.cloudfront.net/`

Click the "Save" button.

Your site's images should now be proxied and optimized through Cloudinary.


