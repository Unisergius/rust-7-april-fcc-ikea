# Rust - fCC Meetup in Ikea Algarve - 12th April 2023

  Guidelines to get hands on into Rust.

## Rust is here. Why should I care about it?

  * Concurrency, Safety, Speed. How?
  * Safety **AND** Speed 
  * No Garbage Collector
  * Excellent memory manager sifting the program using Stack and Heap data structuring.
  * [Ownership and Borrow Checker](https://rabingaire.medium.com/memory-management-rust-cf65c8465570) 
  * And other things like being Easy to compile it to WebAssembly, immutability by default, detailed type annotations...

## Ownership and Borrow Checker - A very important concept to understand in RUST

* [*Ownership is Rust’s most unique feature, and it enables Rust to make memory safety guarantees without needing a garbage collector.*](https://doc.rust-lang.org/book/ch04-00-understanding-ownership.html)
* The rule - a variable can :
  * either have a one mutable reference to it 
  * or multiple immutable references to its data
  * never both.
  * [Example shown in this article](https://blog.logrocket.com/introducing-the-rust-borrow-checker/)
* Borrow checker listens to this rule and gives you compile-time errors indicating you must follow the rule strictly.

## That's too many good news. What's the catch here?

Some of the red dots on Rust.
* All these new paradigms can be a bit complicated and slow you down into creating new stable products 
* Learning curve is steep
* Community has some room to grow
* Get ready for a somewhat ugly syntax.

## But what should I do with Rust exactly? Is it a good language for Start Ups to choose?

  <Explain that this is ultimately a decision that should be in conformity with the vision for the application that needs to be coded>
  
  <Show some production deployed examples done in Rust.>

## Rust Packages Index Website

You can browse Rust Libraries here: 

  * [Rust Crates Registry](https://crates.io/)

## Getting Started

### Requirements 

MacOS needs xcode and corresponding development tools:

```sh
  xcode-select --install
```

Windows: 

* ¯\\_(ツ)_/¯ 

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

Type the following command to update Rust. (Also to check if your terminal recognizes your updated PATH env var)

```sh
  rustup update
```

## What Rust brings to the table


#### Rust compiler is very elaborate in showing you what your program does wrong. 

For example, let's do something we'd usually do on javascript into a file called *im-coding-js-in-rust-lol.rs* .

```rust
  function slapSomeone(yourName, targetName) {
    return yourName + " slaps " + " around a bit with a large trout";
  }
```

Try to compile this. you already know it's not going to run. But see if you can correct the program without resorting any stack overflow shenanigans. Rust compiler should illustrate problems like it's the van gogh of ascii characters.

```sh
  rustc im-coding-js-in-rust-lol.rs
```

#### All variables are immutable by default.

[The value initialized into the variable cannot be changed unless specifically specified.](https://doc.rust-lang.org/book/ch03-01-variables-and-mutability.html)

```rust
fn main() {
    let x = 5;
    println!("The value of x is: {x}");
    x = 6;
    println!("The value of x is: {x}");
}
```

This will give you a compile time error. See if you can make this program work out.

#### [Data Types](https://doc.rust-lang.org/book/ch03-02-data-types.html)

Data types are special annotations that you can specify after the variable. 
They can be inferred by its initial value or you can specifically tell them what they are.

```rust
  let a = 2; //i32
  let b: i32 = 2;
```

The list of types you can annotate are [here](https://doc.rust-lang.org/reference/types.html)

#### Strict scope rules

Like in many modern iteration of languages, for you to use a function you need 
you need to declare that you're using it. You need to include it on the scope you're working.

Example

```rust 
use std::cmp::least;

```

#### Ownership

## What's Next: 

### Rust eBooks

[Rust website](https://www.rust-lang.org/learn) offers you 3 approaches: 

* Book
* Rustlings Course
* By Examples

### Book

[Get book. Must read non-fictional book.](https://doc.rust-lang.org/book/)

This gives your the basics. Instalation, Cargo package manager, your first program with user interaction. And then much much more.

### Rustlings 

Rustlings is an open source project you can clone to do Rust exercises:

* https://github.com/rust-lang/rustlings/

### By Example

A list of examples in Rust, demonstrating most Rust's programming courses .

* https://doc.rust-lang.org/rust-by-example/


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

### Articles about Rust

* https://www.rerun.io/blog/why-rust
* https://blog.logrocket.com/introducing-the-rust-borrow-checker/
* https://www.youtube.com/watch?v=br3GIIQeefY
* https://www.youtube.com/watch?v=oY0XwMOSzq4
