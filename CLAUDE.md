# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repository is

A Claude Code plugin marketplace for Hammersley Futures. There is no application code, build system, or test suite — the repository consists of the marketplace manifest and documentation. Users install it with `/plugin marketplace add HammersleyFutures/marketplace`.

## Structure

- `.claude-plugin/marketplace.json` — the marketplace manifest. Each entry in `plugins` lists a plugin's name, version, description, and source. Plugin code lives in separate repositories referenced by git URL, not in this repo.
- `README.md` — public listing of available plugins; keep it in sync with `marketplace.json` when adding or updating plugins.

## Making changes

When adding or updating a plugin: edit `.claude-plugin/marketplace.json` (bump the plugin's `version` when its source repo changes) and update the matching entry in `README.md`.
