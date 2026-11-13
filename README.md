# Prompt Compare

Run two system prompts or two Claude models on the same inputs and compare answers, speed and cost.
**[Try it live](https://eidos-lab-fr.github.io/prompt-compare/)**


## Features

- Two variants, each with its own model and system prompt
- Any number of test inputs, both variants run in parallel on each
- Time to first token, total time, tokens and estimated cost per answer
- Summary table and CSV export of every run

## Usage

Open `index.html` in a browser, paste an [Anthropic API key](https://console.anthropic.com/), and run it. There is nothing to install and nothing to build.

## Your key, your cost

This page has no server. It calls the Anthropic API straight from your browser with **your own key**:

- The key is kept in the browser tab, or on the device if you tick "Remember". It is sent only to `api.anthropic.com`.
- Nobody else's key is involved, so hosting this page publicly costs its owner nothing.
- Each run shows the tokens used and an estimated cost. Use a key with a spending limit.

The Anthropic SDK is loaded from `esm.sh` at a pinned version. You can choose between Claude Opus 5.5, Sonnet 5.5 and Haiku 5.5.

A comparison makes one API call per input and per variant.

## Stack

A single HTML file. Anthropic TypeScript SDK loaded as an ES module.

## License

[MIT](LICENSE) © 2026 Eidos Lab
