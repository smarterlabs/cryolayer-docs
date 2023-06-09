---
sidebar_position: 1
slug: /configuration
---

# Configuration

The following options are available in the `config.js` file:

## `webflowUrls`

An object of Webflow URLs to proxy. The key is the path where the site will be available, and the value is the Webflow URL. For example, if you want to proxy `https://example.com` at `https://example.org`, you would set `webflowUrls` to `{ "/": "https://example.com" }`.

## `canonical`

The canonical URL of your site. This is used to generate the `canonical` meta tag and the `sitemap.xml` file.

## `removeWebflowJs`

Whether to remove the Webflow JS from the site. This offers a major performance boost. Just be aware that some Webflow features may not work without the JS. This includes hamburger menus, tabs, sliders, forms, and animations.

## `robotsTxt`

The contents of the `robots.txt` file. Leave empty to allow Google to crawl your site.

## `sitemapXml`

The contents of the `sitemap.xml` file. Exclude this property to automatically generate a sitemap from your Webflow sites.

## `cloudinaryImages`

Whether to proxy images through Cloudinary. This allows you to use Cloudinary's image optimization features. You must set the `cloudinaryCloudName` property for this to work.

## `imagePath`

The Cloudinary proxy path to use for images. See the [Cloudinary](/cloudinary) page for more info on Cloudinary configuration.

## `imageFormat`

The Cloudinary transform parameters to use. By default it is set up to automatically compress and convert your images to WebP if the user's browser supports it. See the [Cloudinary docs](https://cloudinary.com/documentation/transformation_reference) for more info.


## `cloudinaryMapping`

A mapping of Webflow image URLs to Cloudinary image URLs. This is used to proxy images that are hosted on Webflow's proxy. At the time of writing it is set to proxy images from the Webflow CDNs that are available. However if you notice your images aren't being proxied, you can add the Webflow domain here.