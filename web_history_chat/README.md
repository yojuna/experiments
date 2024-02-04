## Overview

Local LLM chat over your browser history. Choose relevant files from your web surfing history and pass it to a local version of an llm to chat with it.

Basic POC with separate pieces.

## Dev Notes

- setup the firefox/chrome extension that reads from your browser's history.
    - using open source firefox extension [firefox-better-history-ng](https://github.com/Christoph-Wagner/firefox-better-history-ng)
        - Project description: A history interface inspired by Vivaldi.
            This extension brings a new page to browse your history. It contains 3 views: a daily, weekly and monthly view. If Dark mode is enabled in your OS settings, the dark theme is automatically enabled. Addon page: https://addons.mozilla.org/en-US/firefox/addon/firefox-better-history/

- Get the list of links that are relevant (or all from a specific time period)

- Get the web page content from the list of links

- Local LLM RAG setup that uses extracted web page data, passes it to the embedding/vector store.

- Chat with your history

- Make the flow end to end.

- Select specific links from the time range before exporting/sending to the llm.

## Motivation

Personal digital gardens will make a comeback as it is becoming abundantly clear that models trained on your specific data yield better responses.

First step towards that.

Instead of a digital garden, here using basic links for web pages and seeing how the POC works.

