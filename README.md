# Medusa
Medusa is a portfolio theme for ![Pico CMS](http://picocms.org/) built with ![Boba](https://www.buildwithboba.com/docs/index.html) css framework. 

## Config
Change the `config.yml` file inside pico's `config/` folder
```
##
# Basic
##
site_title: Medusa                                      # The title of your website
base_url: ~                                             # Pico will try to guess its base URL, if this fails, override it here
description: Personal photo diary                      # Set description of website
keywords: photo, portfolio, diary, photodiary           # Set keywords for SEO
author: Andrea B.                                       # Set author of website
robots: index,nofollow                                  # Se robots for all website
favicon: favicon-32x32.png                              # set the name of your favicon                     
rewrite_url: ~                                          # A boolean (true or false) indicating whether URL rewriting is forced
timezone: UTC                                           # Your PHP installation might require you to manually specify a timezone
footer_text: Copyright 2019 to Medusa - All rights reserved     # Set footer text

##
# Theme
##
theme: medusa                                           # The name of your custom theme
theme_url: ~                                            # Pico will try to guess the URL to the themes dir of your installation
                                                        # If this fails, override it here. Example: http://example.com/pico/themes/
twig_config:
    cache: false                                        # Enable Twig template caching by specifying a path to a writable directory
    autoescape: false                                   # Let Twig escape variables by default
    debug: false                                        # Enable Twig's debugging mode
    
theme_config:
    link_color: green                                   # Set links color, options: red, orange, yellow, green, teal, blue, indigo, purple, pink
    name_link_menu: true                                # Set true if you want to show title menu instead of date
    pagination_number: 5                                # Se number of posts display in homepage, default to 5

##
# Content
##
date_format: %d %b %Y               # Pico's default date format
                                    #     See http://php.net/manual/en/function.strftime.php for more info
pages_order_by_meta: author         # Sort pages by meta value "author" (set "pages_order_by" to "meta")
pages_order_by: date                # Change how Pico sorts pages ("alpha" for alphabetical order, "date", or "meta")
pages_order: asc                    # Sort pages in ascending ("asc") or descending ("desc") order
content_dir: content/               # The path to Pico's content directory
content_ext: .md                    # The file extension of your Markdown files
content_config:
    extra: true                     # Use the Parsedown Extra parser to support extended markup
                                    #     See https://michelf.ca/projects/php-markdown/extra/ for more info
    breaks: false                   # A boolean indicating whether breaks in the markup should be reflected in the
                                    #     parsed contents of the page
    escape: false                   # Escape HTML markup in your content files; don't confuse this with some sort of
                                    #     safe mode, enabling this doesn't allow you to process untrusted user input!
    auto_urls: true                 # Automatically link URLs found in your markup

##
# Plugins
##
DummyPlugin.enabled: false          # Force the plugin "DummyPlugin" to be disabled

##
# Custom
##
#intro: Welcome to my portfolio    

```
