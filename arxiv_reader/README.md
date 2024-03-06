# arxiv reader mobile web app

At this point, have hundreds of downloaded arxiv papers in my phone's downloads folder. Metadata of the files is not handled well by the existing pdf reader apps i use (drive, pocketbook). Downloaded papers get lost due to this after a few days. Hoping to resolve that problem.
Existing open source apps are not exactly designed for this specific purpose. Long time obsession, finally jotting down.

Nothing fancy, just a mobile web app that locally reads the papers on the filesystem. Renames or tags the downloaded pdf and creates a directory listing for easier access and reference.

## steps

- Create a mobile PWA app using pdf.js that parses the metadata from the pdf file and renames + organizes the papers donwloaded locally.
- If possible, include arxiv sanity functionality as well.
- Extend to papers downloaded from any source.
- open source PWA mobile app, run completely locally.

## refs/links:

- [gh: mozilla/pdf.js](https://github.com/mozilla/pdf.js)
- [gh: tchittesh/arxiv-viewer](https://github.com/tchittesh/arxiv-viewer)
    - pdf.js fork for arxiv; might be useful for bootstrapping

- [gh: GarrettBeatty/arXiv-eXplorer](https://github.com/GarrettBeatty/arXiv-eXplorer)
    - android app for arxiv papers
    - have tried this personally, good but doesn't exactly scratch the itch

- [gh: karpathy/arxiv-sanity-preserver](https://github.com/karpathy/arxiv-sanity-preserver)