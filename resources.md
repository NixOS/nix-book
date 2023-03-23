# Current state of documentation

> ![](https://documentation.divio.com/_images/overview.png)
>
> [The documentation system](https://documentation.divio.com/), a framework to think about various types of documentation, each with their own purpose and capabilities.

When viewed in the framework of [The documentation system](https://documentation.divio.com), we observe the following.

The manuals appear not to be maintained in any coordinated fashion, supposedly due to their ever increasing size. They do not serve a clear-cut purpose, and are instead somewhere in between an explanation and a reference, fulfilling both roles only partially.

There exist many resources showing *how to use* Nix or NixOS or interact with `nixpkgs`, some in writing, some as instructional videos.

There exists an overwhelming amount of “Nix” explanations, all of which *only* refer to the Nix configuration language.

There seems to exist no self-contained, complete, up-to-date **explanation** of Nix the package manager, NixOS, or `nixpkgs` with respect to fundamental operating principles, architecture and design decisions! @edolstra’s thesis is still the most comprehensive source on rationale, yet only covers Nix language and package manager in depth.

Given [the thesis has been removed from the NixOS web site in 2017](https://github.com/NixOS/nixos-homepage/issues/830), we can assume that more recent Nix newcomers do not even know it exists. As the thesis is not a living document, it is necessarily outdated in some regards. It still has the most precise conceptual explanations, and presenting them in accessible form would already improve the state of affairs.

<table><tr valign=top><td>

### Tutorials

Nix language
- [learn Nix in Y minutes](https://learnxinyminutes.com/docs/nix/)
- [Tour of Nix](https://nixcloud.io/tour/?id=1)
- [Nix by example](https://medium.com/@MrJamesFisher/nix-by-example-a0063a1a4c55)
- [Nix Language Overview](https://www.youtube.com/watch?v=eCapIx9heBw&amp;list=PL-saUBvIJzOkjAw_vOac75v-x6EzNzZq-&amp;index=5)
- [Nix Pills Chapter 4](https://nixos.org/guides/nix-pills/basics-of-language.html) and [5](https://nixos.org/guides/nix-pills/functions-and-imports.html)

Nixpkgs
- [Nix Shell Overview](https://www.youtube.com/watch?v=SGekN4pDExY&amp;list=PL-saUBvIJzOkjAw_vOac75v-x6EzNzZq-&amp;index=6)
- [Nix Fundamentals](https://www.youtube.com/watch?v=m4sv2M9jRLg)
- [Nix Pills Chapter 8](https://nixos.org/guides/nix-pills/generic-builders.html), [9](https://nixos.org/guides/nix-pills/automatic-runtime-dependencies.html), [10](https://nixos.org/guides/nix-pills/developing-with-nix-shell.html), [12](https://nixos.org/guides/nix-pills/inputs-design-pattern.html), [13](https://nixos.org/guides/nix-pills/callpackage-design-pattern.html), [14](https://nixos.org/guides/nix-pills/override-design-pattern.html), [16](https://nixos.org/guides/nix-pills/nixpkgs-parameters.html), [17](https://nixos.org/guides/nix-pills/nixpkgs-overriding-packages.html), [19](https://nixos.org/guides/nix-pills/fundamentals-of-stdenv.html), [20](https://nixos.org/guides/nix-pills/basic-dependencies-and-hooks.html)

NixOS
- [NixOS Filesystem Overview](https://www.youtube.com/watch?v=jf0nIn2oS8A&amp;list=PL-saUBvIJzOkjAw_vOac75v-x6EzNzZq-&amp;index=4)

Nix package manager
- [Nix Pills Chapter 3](https://nixos.org/guides/nix-pills/enter-environment.html), [6](https://nixos.org/guides/nix-pills/our-first-derivation.html), [7](https://nixos.org/guides/nix-pills/working-derivation.html), [11](https://nixos.org/guides/nix-pills/garbage-collector.html), [15](https://nixos.org/guides/nix-pills/nix-search-paths.html), [18](https://nixos.org/guides/nix-pills/nix-store-paths.html)
</td>
<td>

### How-To Guides

Nix language

Nixpkgs
- [NixOS Wiki FAQ](https://nixos.wiki/wiki/FAQ)
- [nix.dev guides](https://nix.dev/)
- [Jon Ringer’s videos](https://www.youtube.com/channel/UC-cY3DcYladGdFQWIKL90SQ)
- [Nixpkgs manual](https://nixos.org/manual/nixpkgs/stable)

NixOS
- [nix.dev guides](https://nix.dev/)
- [Jon Ringer’s videos](https://www.youtube.com/channel/UC-cY3DcYladGdFQWIKL90SQ)
- [Nix notes](https://github.com/noteed/nix-notes)
- [NixOS Manual](https://nixos.org/manual/nixos/stable/)

Nix package manager
- [NixOS Wiki: Managing the Store](https://nixos.wiki/wiki/Nix_Cookbook#Managing_storage)</td></tr><tr valign=top><td>

### Explanation

Nix language

- [PhD Thesis](https://edolstra.github.io/pubs/phd-thesis.pdf)

Nixpkgs
- [Nix Pills, partial](https://nixos.org/guides/nix-pills/index.html)
- [Connecting Bash to Nix](https://www.zombiezen.com/blog/2023/03/connecting-bash-to-nix/)

NixOS

Nix package manager
- [PhD Thesis](https://edolstra.github.io/pubs/phd-thesis.pdf)</td><td>

### Reference

Nix language
- [PhD Thesis](https://edolstra.github.io/pubs/phd-thesis.pdf)
- [Nix manual (writing Nix expressions)](https://nixos.org/manual/nix/stable/expressions/writing-nix-expressions.html)
- [one-page reference](https://github.com/tazjin/nix-1p)

Nixpkgs
- [Nixpkgs manual](https://nixos.org/manual/nixpkgs/stable)

NixOS
- [NixOS manual](https://nixos.org/manual/nixos/stable)

Nix package manager
- [PhD Thesis](https://edolstra.github.io/pubs/phd-thesis.pdf)
- [Nix manual (command reference)](https://nixos.org/manual/nix/stable/command-ref/command-ref.html)
</td></tr></table>


> Note that we have significantly more how-to material than anything else, which does not show prominently in the table because is summarized in NixOS Wiki and nix.dev.
