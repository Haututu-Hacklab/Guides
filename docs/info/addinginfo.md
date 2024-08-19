# Documentation

## Framework

This documentation is built using [mkdocs](https://www.mkdocs.org).

## Submitting Content

Please see the [repository readme](https://github.com/Haututu-Hacklab/Guides/blob/main/README.md) for information on submitting content for the site.

## Project layout

    mkdocs.yml    # The configuration file for the site itself.
    assets/
        ... # Files to be included in other pages that shouldn't be directly accessible themselves.
    docs/
        index.md  # The documentation homepage.
        ...       # Other top-level markdown pages, including explanations of each Ombi UI page.
        assets/
            images/
                embeds/
                    ... # Images for use in pages
                hacklab/
                    ... # Official Hacklab images (logos etc).
        guides/
            ... # Any markdown page classified as a 'guide' (like how to do something with something etc)
            3dprinting/
                ... # Guides for the 3d printers 
            laser/
                ... # Guides for the laser cutter  
        info/
            ... # Any markdown page that falls under the 'info' category (info about the hacklab, info about the documentation site, technical information about the hardware itself)
        settings/
            ... # Markdown pages explaining each specific settings page
            notifications/
                ... # Markdown pages explaining each notification setting page 
