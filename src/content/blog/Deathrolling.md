---
title: 'Deathrolling - WASM implementation of a game'
description: 'A webassembly implementation of a gambling game found in WoW.'
pubDate: 'Sep 23 2022'
heroImage: '/Deathrolling.png'
tags: ["Rust"]
---
## Summary

This website is a Rust and webassembly implementation of the gambling game from WoW.
The game is not that complex, but is hard to explain so lets go through an example game.

Two players have decided to bet 10 dollars and the winner will be decided by playing a game of deathrolling.
The two players choose a number as their starting number, lets say they choose 500.
The first of the two players then rolls a number between 1 and the current number, which is 500.
The result is the number 353.
The second player then rolls a number between 1 and this new number, which is 353.
This continues until one of the two players roll a 1.

To play the game on this website, you enter a number and take turns to click on the screen to trigger a roll. The first person to roll a 1 is the loser.

The main technology used is a web framework by the name Yew, which is a react like framework.
The purpose of this project was to try out Rust and see how far web development had come with Rust and WASM.
The developer experience was good, but the documentation left something to be desired.
It did leave me wanting to do more Rust development, which later led into the WebGPU project seen [here](https://madswolf.dk/projects/webgpu).

## Links

The projects code can be found [here](https://www.github.com/madswolf/deathrolling) and a live version of the site can be found [here](https://deathrolling.madswolf.dk/).
