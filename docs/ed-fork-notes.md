# Ed's LÖVE fork notes

This repository is a fork of the LÖVE engine source, not a normal `main.lua` game project.

## Current purpose

Use this fork as the engine-side experiment branch for the top-down dungeon crawler project.

For now, engine behavior should stay untouched unless a change gives the game project a clear advantage, such as:

- debugging hooks that help inspect Love2D runtime behavior;
- project-specific build notes for Windows;
- clean examples showing how the crawler should be launched against this fork;
- small, reversible engine experiments that are isolated and easy to remove.

## Working rule

Do not casually modify core engine files just to make game features. The crawler itself should live in a separate Love2D game repo or folder with `main.lua`, `conf.lua`, assets, and Lua modules.

Only change the engine when the normal Love2D API is genuinely blocking the project.

## First safe checkpoint

This file exists to mark the fork as project-owned and to give future commits a sane direction before any C++ engine changes are made.
