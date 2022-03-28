# The Orbital Widget Toolkit

[<img src="img/orbtk_planet.svg" width="720"/>](img/orbtk_planet.svg)

*by Florian Blasius, with contributions from the Rust Community*

*annotated and documented by Ralf Zerres and all contributers*

This version of the text assumes you’re using OrbTk v0.3.1 or later in
conjuction with Rust v1.59.0 or later. *Cargo.toml* should define
`edition="2018"`. That enables and uses Rust 2018 Edition idioms in
all derived projects.

See the [“Installation” section of Chapter 1][install]
to install or update OrbTk.

The 2020 Edition of this book is the initial release. It will be
released with the OrbTk version 0.3.1.

- Appendix A “Keywords”, explains the new raw identifiers.
- Appendix D “Translations”, is work in progress. We will release
  instances of this book in the target language once they are translated.

For online reading, a HTML rendered version is available at [Orbtk
book][orbtk_book_en]. Alternatively you might want to have it handy
for offline usage. Either you downlaod a rendered `pdf` or
`ebook`version or go ahead and download the source. Then kick on
mdbook (the definition of the target location is optional).

We try hard, to make this book available in multiple languages. As a
consequence, the source directory is structured to serve [localized
subdirectories][mdbook_localization].  Thus to render its contents you
need an enhanced version of mdbook. [Ruin0x11][mdbook_branch] is
maintaining a git branch **localization**, a [PR][mdbook_pr_1306] is commited upstream.

[mdbook_localization]: https://github.com/Ruin0x11/mdBook/tree/localization
[mdbook_branch]: https://github.com/Ruin0x11/mdBook.git
[mdbook_pr_1306]: https://github.com/rust-lang/mdBook/pull/1306

Go ahead and install that mdBook version like this:

```console
TMPDIR=<your_temporary_directory>
mkdir -p $TMPDIR; cd $TMPDIR
git clone https://github.com/Ruin0x11/mdBook.git
cd mdBook
git checkout localization
cargo update
cargo install --path .
```

To download and compile the orbkt-book source, please use the following commands:

```console
TMPDIR=<your_temporary_directory>
mkdir -p $TMPDIR; cd $TMPDIR
git clone https://github.com/redox-os/orbtk-book.git
cd orbtk-book
mdbook build --language en --dest-dir doc/book_en --open
```

<!---
This text is available in [paperback and ebook format from No Starch Press][nsprust].
-->

[install]: https://doc.redox-os.org/orbtk-book/ch01-01-installation.html
[nsprust]: https://nostarch.com/orbtk
[orbtk_book_en]: https://doc.redox-os.org/orbtk-book/index.html

<!--
[orbtk_book_en]: https://github.com/redox-os/orbtk-book
[orbtk_book_en_stable]: https://doc.orbtk.org/stable/book_en/html/print.html

-->
