# Rust - fCC Meetup in Ikea Algarve - 12th April 2023

  Guidelines to get hands on into Rust.

## Rust is here. Why should I care about it?

  <Get the good points about Rust here>

## That's too many good news. What's the catch here?
  
  <Get some bad points about Rust here>

## But what should I do with Rust exactly? Is it a good language for Start Ups to choose?

  <Explain that this is ultimately a decision that should be in conformity with the vision for the application that needs to be coded>
  
  <Show some production deployed examples done in Rust.>
  

## Getting Started

### Requirements 

MacOS needs xcode and corresponding development tools:

```sh
  xcode-select --install
```

Windows: 

* ¯\_(ツ)_/¯ 

Linux needs gcc installed. Depending on your system package manager you'll probably have the package gcc available to install.

APT Example : 

```sh 
  sudo apt install gcc
```


## Install Rust 

This fetches the installer and pipes the downloaded file into executing it.
It will install Rust and Cargo. Cargo is Rust's package manager.

```sh
  curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh 
```


By the end the installer will show you this message:

```sh
Rust is installed now. Great!

To get started you may need to restart your current shell.
This would reload your PATH environment variable to include
Cargo's bin directory ($HOME/.cargo/bin).

To configure your current shell, run:
source "$HOME/.cargo/env"
```

It's important that your path recognizes Rust folder for executables "bin". 
So if you're command lines are not being recognized, please check your 
PATH env variable.

## Update Rust

Type the following command to update Rust.

```sh
  rustup update
```

## What's Next: 

### Rust eBooks

Rust website offers you 3 approaches: 

* 

### Rustlings 

Rustlings is an open source project you can clone to do Rust exercises:

* https://github.com/rust-lang/rustlings/

### HackerRank

After these exercises you can start doing basic HackerRank exercises to up your Rust face on:

* [HackerRank Algorithm Exercises (Must Choose Rust Language)] https://www.hackerrank.com/domains/algorithms

## Rust Frameworks

### Actix Web - Web Framework

* [Actix Web Github repo](https://github.com/actix/actix-web)
* [Community Showcase](https://github.com/actix/examples#readme)
* [Getting Started](https://actix.rs/docs/getting-started)

### Axum - Web Framework

* [Axum Github Repo](https://github.com/tokio-rs/axum)

### Yew - Frontend Framework

* [Yew Github Repo](https://github.com/yewstack/yew)

### Rocket - Web Framework

* [Rocket Github repo](https://github.com/SergioBenitez/Rocket)
* [QuickStart](https://rocket.rs/v0.5-rc/guide/quickstart/)

### Web Framework Listings 

* [Flosse's web frameworks and libs written in Rust](https://github.com/flosse/rust-web-framework-comparison)

### Bevy - Game Engine

* [Bevy Github Repo](https://github.com/bevyengine/bevy)

### Amethyst - Game Engine

* [Amethyst Github Repo](https://github.com/amethyst/amethyst)

### List of Game Engines

* [Arewegameyet.rs](https://arewegameyet.rs/ecosystem/engines/)

## Rust Project

### Building a calculator in Rust

* [FreeCodeCamp's Rust in Resplit](https://www.freecodecamp.org/news/rust-in-replit/#how-to-use-rust-in-replit)
