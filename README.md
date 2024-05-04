# Dictionary Web App - Frontend Mentor Challenge

This is a solution to the [Dictionary Web App](https://www.frontendmentor.io/challenges/dictionary-web-app-h5wwnyuKFL). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)

  - [The challenge](#the-challenge)

- [My process](#my-process)

  - [Built with](#built-with)

- [Author](#author)

## Overview

### The challenge

This challenge requires calling an api to retrieve dictionary word definitions and displaying them. The api chosen for this is [dictionaryapi.dev](https://dictionaryapi.dev).

This is a simple api call with a somewhat challenging response format. It is based on wikitext which is freeform, so there are often inconsistencies in the json that is returned, depending on word. For example, the audio file reference may be in second or third pronunciation slot in the returned array depending on what the article author did on wiktionary.

Themes throws in a new wrinkle with font themes of Sans-serif, Serif, Monospaced, along with the more typical day/night color scheme switching. Automatic system switching is also implemented.

An `<audio>` element is required in order to play mp3, ogg, etc. for the word pronunciation. The custom button requires that the audio element have controls hidden and be controlled through api only.

The web page must be fully accessible and support full keyboard navigation. This requires a custom dropdown menu implementation with appropriate aria usage to replace the intrinsic system accessibility normally available in `<select>`.

To add to the utility of the page, permalink hashes are added to the URL. This allows any search to be bookmarked and for back/forward browser navigation to act as a search history.

An accessible busy spinner and live region is used in this implementation. During development, the dictionaryapi.dev site went down for several hours. This forced better error handling, timeout handling etc.

## My process

### Built with

- Next.js 14
- Zod
- Shadcn

## Author

- [LinkedIn](https://www.linkedin.com/in/katlegomabaso/)
