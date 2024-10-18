# Chrome extension template

React, typescript, vite chrome extension template. Currently has a popup, options and injected content react components.


## Why make another chrome extension template?

I found other templates online:
* https://wxt.dev/
* https://github.com/guocaoyi/create-chrome-ext

But I wanted the content script to also use react and I didnt know how to change them
to fit what I wanted. So I created this.

## Folder Structure
* `.config`: Contains vite build configs for each part of the chrome extension
* `build`
  * `build/manifest`: manifest for chrome extension
  * `build/assets`: assets for chrome extension accessible via web accessible resources in manifest
  * Everything else in build is ignored by git. Built chrome extension files go here
* `src`
  * `src/features`: Contains different parts of the chrome extension
    * `src/features/popup`: Contains react app for popup
* `.html`: html files at root are entry points for vite to build.
* `vite.config.base.ts`: Common vite built config for all parts of chrome extension
