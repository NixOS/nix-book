# Contributing to this project

The Nix Book is a community effort to collect, create, and maintain world-class learning resources for Nix.

We strongly encourage everyone interested to contribute by asking informed questions or directly proposing changes.

Open an issue if you want to clarify something not evident from what is provided in this repository, or if you want to discuss a significant change before starting to work on it.

Make a pull request if you want to introduce an incremental change.
Note our [considerations on licensing and attribution](#licensing-and-attribution).

## You want to learn and use Nix?

This book would not be possible without you.
Try to use it as your primary resource, however incomplete it may appear.

We ask you to liberally open issues and document all problems and questions that arise.
Please also state your learning goals and the paths you have taken so far.

Sharing your first-hand experience is invaluable to better guide our efforts, and will immediately help improve the book for yourself and everyone else.

## You have experience teaching Nix?

You will probably have observed where learners get stuck most often, and which typical needs and questions they have.
You may have your own written notes for classes, trainings, or presentations.

Please share your experience and help us inform the structure and detailed contents of this book.
It would be great if you could contribute examples, wordings, or illustrations that proved helpful to your students.

## You are a domain expert using Nix?

If you are proficient in applying Nix to a domain-specific problem, and want to share your expertise on best practices, please check the table of contents.
Does existing material on your subject meet your standards?
How could we improve it?
Is there a popular application of Nix' capabilities not yet covered?
We would be glad to incorporate your insights.

# Guidelines

Here are values and practical guidelines to go by when contributing.

## Values

### Be kind

Adapted from [Contributor Covenant](contributor-covenant) and [The Carpentries Code of Conduct](carpentries-coc):

- Use welcoming and inclusive language
- Show empathy and respect towards other people
- Be respectful of different viewpoints and experiences
- Give and gracefully accept constructive criticism
- Focus on what is best for the community

[contributor-covenant]: https://github.com/EthicalSource/contributor_covenant/blob/cd7fcf684249786b7f7d47ba49c23a6bcb3233eb/content/version/2/1/code_of_conduct.md?plain=1#L25-L31
[carpentries-coc]: https://github.com/carpentries/docs.carpentries.org/blob/4691971d9f49544054410334140a4fd391a738da/topic_folders/policies/code-of-conduct.md?plain=1#L15-L19

### Be truthful

The only thing more confusing than no documentation is misleading documentation.

#### Use and provide evidence

This book should enable readers to answer all their questions on their own.

Provide [links](#links) to the [online Nix manual][nix-manual] or other resources, if it would help guide readers on their learning journey.
It is explicitly within scope of this project, and encouraged by Nix maintainers, to update or restructure the [Nix manual source code][nix-manual-src] where appropriate, to improve the overall experience.

Similarly, the other information in this repository should enable contributors to answer most of their questions and correct obvious errors on their own, and only then resort to opening issues.

Errors get more obvious if we can measure execution against intent.
Therefore we ask you to always make explicit the motivation behind your proposed changes.

Add references to any relevant resources in commit messages, if it helps understand the reasoning behind a significant change.

[nix-manual]: https://nixos.org/manual/nix/stable/
[nix-manual-src]: https://github.com/NixOS/nix/tree/master/doc/manual

#### Ensure working code samples

Code samples must always be working correctly when run as instructed.
Nix provides us with everything needed to make this happen.

Currently we have no automated tooling in place to assist with this, and pull requests to address that question are very welcome.

### Be concise

> I would have written a shorter letter, but I did not have the time.
>
> — [Blaise Pascal][shorter-letter]

This book is for the readers, and their time and attention is limited.
Take the time to be extraordinarily respectful with their cognitive resources.

You can use diagrams or illustrations to support written descriptions.
[GitHub allows creating Mermaid diagrams within Markdown.][github-mermaid]

The same holds for communication directed to contributors and maintainers:
This is a public project, and many people will read what you write.
Use this leverage with care.

[shorter-letter]: https://en.m.wikiquote.org/w/index.php?title=Blaise_Pascal&oldid=2978584#Quotes
[github-mermaid]: https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/

## Guides

### File organization

```
├── README.md       | project front page on GitHub
├── CONTRIBUTING.md | this file
├── LICENSE.md      | license information
├── resources.md    | categorized collection of existing learning resources
└── src             | book contents
```

### Licensing and attribution

When opening pull requests with your own contributions, you agree to licensing your work under [CC-BY-SA 4.0][cc-by-sa].
You will be considered co-author of this book, as recorded by version history.

When adding material by third parties, make sure it has a matching license that permits this.
In that case, [unambiguously](#links) state source, authors, and license.
Also [add the original author as co-author][github-multiple-authors] to the respective change, so we can track authorship through version history.

Notify the authors *before* using their work.

[cc-by-sa]: https://creativecommons.org/licenses/by-sa/4.0/
[github-multiple-authors]: https://docs.github.com/en/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/creating-a-commit-with-multiple-authors

### Links

Unless explicitly required to point to the latest version of an external resource, all references should be [permanent links][permalink].

Many web services offer permalinks.
Examples:
- [GitHub URLs to specific commits][github-permalink]
- [Wikipedia URLs to specific page versions][wikipedia-permalink]
- [Internet Archive "Save Page Now" for persisting web pages][internet-archive-save]

[permalink]: https://en.m.wikipedia.org/wiki/Permalink
[github-permalink]: https://docs.github.com/en/repositories/working-with-files/using-files/getting-permanent-links-to-files
[wikipedia-permalink]: https://en.m.wikipedia.org/wiki/Wikipedia:Linking_to_Wikipedia#Permanent_links_to_old_versions_of_pages
[internet-archive-save]: https://web.archive.org/save

### Markdown

Write one sentence per line.
This makes it easier to manage changes.
The rule is unambiguous and does not require tooling support to be applied easily.

[Here is a discussion of different line wrapping styles.][markdown-wrapping-styles]

[markdown-wrapping-styles]: https://web.archive.org/web/20220519121408/https://mtsknn.fi/blog/4-1-wrapping-styles-for-markdown-prose-and-code-comments/
