---
title: 'Deathrolling in WASM'
description: 'A webassembly implementation of a gambling game found in WoW.'
pubDate: 'Sep 23 2022'
heroImage: '/Deathroll.png'
tags: ["Rust"]
---
## Summary

This website is a Rust and webassembly implementation of the gambling game from WoW.
The game is not that complex, but is hard to explain so lets go through an example game.

## Understanding Deathrolling

Two players agree to bet a certain amount, say $10, and decide the winner through a game of Deathrolling. They start by choosing an initial number, for instance, 500.

- First Roll: Player 1 rolls a random number between 1 and 500, resulting in 353.
- Second Roll: Player 2 then rolls a random number between 1 and 353.
- Subsequent Rolls: The players continue this process, each rolling a number between 1 and the most recent roll result.
- Game End: The game continues until a player rolls a 1, at which point that player loses, and the other player wins the bet.

To play the game on this website, you enter a number and take turns to click on the screen to trigger a roll. The first person to roll a 1 is the loser.

## Insights

The implementation leverages Yew, a React-like web framework for Rust. The project aimed to explore Rust's capabilities in web development with WASM. While the developer experience was generally positive, the documentation for these technologies could be improved.

It did leave me wanting to do more Rust development, which later led into the WebGPU project seen [here](https://madswolf.dk/projects/webgpu).

## Links

The projects code can be found [here](https://www.github.com/madswolf/deathrolling) and a live version of the site can be found [here](https://deathrolling.madswolf.dk/).
