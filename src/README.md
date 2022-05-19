# Outline

The book shall be organized top-down from defining a problem domain, the solution approach Nix takes, following explanations how solutions for each specific problems are designed. Each section shall have working examples how to use the presented solution and links to relevant reference manuals.

Each section should have an interactive questionnaire to (at least shallowly) determine learning success and collect feedback.

Sections are ordered from generic to specific. Sections depend on insights from previous chapters, and these dependencies should be made clear, already in the process of developing the book, to further inform a suitable structure or reading order.

Software developers building their own projects may take a different path than end-users who just want to use packaged software temporarily or persistently.

## Which problems Nix solves

- having complete, automatic build instructions
- avoiding dependency hell
- hooking build results into the operating system to make them usable

## How Nix works

Explain high-level architecture, general mechanism, and design rationale of Nix.

- build system
- configuration language
- package manager

@edolstra proposed this to be an appendix. I am convinced a novel paradigm mandates explaining the mechanism first and only then going into details how it applies to specific problems. This chapter should be very concise and make clear the underpinnings, and prominently show diagrams to illustrate the principle. Detailed explanations can follow in chapters on individual subjects.

Also ultimately, in a hypertext document we don't really care about order, and we can always direct the reader by noting what is to be expected from reading a certain chapter.

## What Nix can do

Each section here should start out with a problem description, and explain the mechanism built on top of Nix to solve that problem. Then there should be concrete examples mapping from the explained concepts to interacting with the actual implementation.

### prerequisites

- install Nix

### build and run software

Show how existing build plans are used to produce working software.

- find packaged software
- run software from existing packages
- set up a temporary environment

### package management

This chapter is about how to hold onto the ephemeral examples from the previous chapter, and how to create more complex environments by composing existing packages.

#### imperative package management

Describes a straightforward transition from temporary environments using existing packages.

- persist packages in the file system
- updates, rollbacks, pinning
- garbage collection

Imperative package management's unique feature is that it allows updating each package independently to the most recent available version without touching the rest of the system.

#### declarative package management

While imperative package management supports "generations", it does not have proper change management, "profiles" are not portable, and it is not possible to compose packages into a larger unit.
This section shows how to have all of that by declaring a Nix expression in a file.

- declare a reproducible environment
- compose packages
- adapt packages to your needs

This chapter should have at least a reference to or a full-blown copy of a good introduction to the Nix langauge as a prerequisite for working through examples.
Another option would be to develop an approach to the language by motivating language features through the examples themselves, but that would probably be a lot more work.

### maintain package collection

Explain how existing packages come into being, how their collection is organized, and show how to modify and create packages.

- organization of package collection
- modify existing package
- create new package
- contribute to public repository

Creating packages and contributing are advanced topics that require much more detail (especially langauge specifics), and are partially covered in the `nixpkgs` manual already.
In this context they are intended to demonstrate `nixpkgs` architecture and design, to enable readers to navigate existing code, assess pull requests, and create or maintain their own packages.
This should be fairly superficial, otherwise it would duplicate much of the `nixpkgs` manual.
Alternatively these sections could be dropped entirely, or moved to their own chapter and reference or reuse much of the `nixpkgs` manual.

Another problem with all of the `nixpkgs` topics is that many design questions are still under debate, and implementation is a moving target, even if slowly.
It is not yet clear to me how to deal with this, it seems like a lot of work, and possibly `nixpkgs` is entirely out of scope of this book if we cannot gather enough humanpower to sort through all of that.

### declarative configuration management

Show how the disconnected packages from previous examples can be wired up into a consistent and persistent user environment or operating system configuration.

- user environments
- operating system distribution
- service management

@thufschmitt correctly pointed out that tools like `home-manager` and `nix-darwin` are not "official" Nix projects. He uttered concern that discussing them in this book in depth may touch a political issue: Do they become "blessed" by including them?

My stance on this is that they are mature and widely used tools. They should be discussed right next to NixOS already on the principle that they all depend on `nixpkgs` and the way they work is almost identical, illustrating that the mechanism Nix provides is straighforward.

What is not as clear to me is how to determine if and how alternative contenders should be mentioned. There should be some criteria that makes an alternative approach viable enough to discuss, for example being mature enough to reliably support meaningful examples. Another instance that immediately comes to mind are NixOps and Disnix, both of which (to me) have unclear state of maturity and maintenance, but seem to be developed enough and have interesting concepts that I think are worth including.

### software development

- continuous integration
- distributed builds
- caching
- deployment
- cross-compilation
- bundling build results
    - virtual machines
    - docker containers

