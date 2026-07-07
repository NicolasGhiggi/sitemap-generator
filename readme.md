# Sitemap Generator

Sitemap Generator is a lightweight Python tool that crawls a website and automatically generates XML sitemap files compliant with the Sitemap Protocol.

The crawler starts from a given URL, discovers all internal links within the same domain, and exports them into one or more sitemap files. To improve organization and comply with search engine recommendations, each sitemap contains a maximum of **10,000 URLs**.

## Features

* Crawl an entire website starting from a single URL
* Discover internal links automatically
* Generate XML sitemaps compatible with search engines
* Split large websites into multiple sitemap files (10,000 URLs per file)
* Automatically create a timestamped output folder inside the Downloads directory
* Pretty-formatted XML output
* Simple command-line interface

## Technologies

* Python 3.12+
* requests
* BeautifulSoup4
* xml.etree.ElementTree
* xml.dom.minidom

## Usage

```bash
py sitemap_generator.py
```

Then enter the website URL when prompted:

```text
https://example.com
```

Generated sitemap files will be saved inside:

```text
Downloads/
└── sitemap_files_dd-mm-yyyy_hh-mm-ss/
    ├── sitemap_1.xml
    ├── sitemap_2.xml
    └── ...
```
