# List of third-party add-ons

This repository is a public list of 3rd party integrations of the Tinify image optimization API (https://tinypng.com/developers) with other software.

The list is also published every once in a while at https://tinypng.com/third-party.

## Adding your integration to the list

1. Fork this repository
2. Add a file named `{platform}-{integration name}.md` following requirements below.
3. Create a pull request.

## Requirements

The file name must be formatted as **`{platform}-{integration name}.md`** and entirely lower case. The `platform` corresponds to the `platform` field in the file itself. The `integration name` can be a short name of your integration.

The file contains two parts:
1. Structured YAML "front-matter" with some metadata.
2. A short description of the integration.

### Example:

File `wordpress-tiny-compress-images.md`:

```
---
collection: "Content management"
platform: "WordPress"
type: "Plugin"
developer: "Tinify"
developer_url: "https://tinypng.com/developers"
price: "Free"
url: "https://wordpress.org/plugins/tiny-compress-images/"
---

Automatically optimizes user-uploaded images immediately or in the background.
It also offers a bulk optimization tool to compress your existing media library.
```

### Fields required in front-matter

#### `collection`

Main category of the integration.

Must be one of:
* `"Content management"` – for integrations with content management systems.
* `"Desktop"` – for desktop software with a GUI.
* `"Development"` – for command line tools, client libraries, integrations with programming languages or frameworks.
* `"E-commerce"` – for integrations with webshops and other e-commerce platforms.

#### `platform`

The platform this integration is made for. Depending on `collection` this will be different. For example:

* For content management systems this is the name of the CMS product.
* For desktop software this is the name of the operating system.
* For development tools this is the name of the programming language or framework.
* For e-commerce integrations this is the name of the e-commerce product.

#### `type`

The type of integration. This should follow the naming convention of the platform that is being integrated with.

For example, integrations with WordPress are officially called "plugins", so the `type` would be `"Plugin"`.

For Magento, an integration is officially called an "extension", so the `type` would be `"Extension"`.

#### `developer`

This is the full name of the software development agency or person that authored and maintains this integration.


#### `developer_url`

This is a link to the homepage of the developer. Preferably this would be a location where users can **contact you** if they have any questions about the integration.

#### `price`

This is either `"Free"` or the price in the main currency that you charge users with, for example: `"$ 19.00"`.

#### `url`

This is the location of the **download page** of the integration. It should describe the integration and offer a way for the user to install or download it in order to add it to their platform.

### Description

The description should contain the **main features** of your integration. For example, whether it supports resizing or preserving metadata, whether it optimizes images in the background, etcetera.

You could also provide more information about how it integrates exactly with the platform. For example, whether it optimizes images when they are uploaded by a user to the CMS, or whether they are optimized when the pages are published.

Please avoid describing what TinyPNG or TinyJPEG is. Feel free to include this information on your download page, though.

We'd prefer if this description is approximately **between 80 and 160 characters**.
