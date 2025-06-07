# Person Schema.org Markup Builder

A simple, static web tool for generating schema.org JSON‑LD snippets that describe a Person. Users fill out a form (including tag/chip inputs for array fields), see a live preview of the JSON‑LD, and can copy the markup for use on any website. It’s quick, dirty, and does the job—like duct tape for your metadata.

## Table of Contents

- [Description](#description)  
- [Planned Features (a.k.a. The Wishlist of Good Intentions)](#planned-features)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Contributing](#contributing)  
- [License](#license)  

## Description

This repository provides a self‑contained static HTML, CSS, and JavaScript application that helps content authors and web developers easily create valid [schema.org](https://schema.org/) Person markup in JSON‑LD format. All form inputs—including arrays like `additionalName`, `sameAs`, and `knowsAbout`—are rendered with a modern tag/chip interface. The output is injected into a `<script type="application/ld+json">` block, which can be copied directly or validated via the [Schema.org Validator](https://validator.schema.org/). This whole thing came out of a mix of curiosity, boredom, and an unhealthy respect for structured data.

You can try it out instantly via the [live demo](https://deltaspark.github.io/Schema-Markup-Builder/).

## Planned Features

- Support for "affiliation" to describe organization relationships.
- Full coverage of all schema.org Person properties (planned incremental rollout).
- Improved UX for selectively adding desired attributes and templates for common patterns.
- Maybe more. I'll get to it when I get to it. Promise!

## Installation

Since this is a static page, you only need to clone or download this repository:

```bash
git clone https://github.com/DeltaSpark/Schema-Markup-Builder.git
cd Schema-Markup-Builder
```

No build tools or server runtime required—just double-click `index.html` like it's 2005 and enjoy the ride.

Or, skip the download entirely and try the [live demo](https://deltaspark.github.io/Schema-Markup-Builder/) on GitHub Pages.

## Usage

1. Open `index.html` in your favorite browser, or just visit the [live demo](https://deltaspark.github.io/Schema-Markup-Builder/) on GitHub Pages.  
2. Fill out the form fields on the left pane.  
3. Observe the live-updated JSON‑LD in the right pane.  
4. Click “Copy to Clipboard” to grab the `<script>` snippet.  
5. Paste the snippet into your site’s HTML (inside `<head>` or `<body>`) and validate at the [Schema.org Validator](https://validator.schema.org/).

## Contributing

Contributions are welcome! Send in a pull request, and we can both pretend I know what I'm doing.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## AI Disclosure

This README and much of the HTML scaffolding were created with help from ChatGPT to speed up prototyping a static-page solution—plus, it was a Friday afternoon, and I had plans.