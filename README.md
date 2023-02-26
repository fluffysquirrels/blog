# Alex Helfet's personal blog

[Site](https://fluffysquirrels.github.io/blog/)  
[Source](https://github.com/fluffysquirrels/blog)

## Getting started

* Install rust, usually with [`rustup`](https://rustup.rs/).

* Install `cobalt`, a static site generator written in Rust.

    ```sh
    cargo install cobalt-bin
    ```

* Install [`watchexec`](https://github.com/watchexec/watchexec) (used by `./bin/preview`)

    ```sh
    cargo install watchexec
    ```

## How to preview

To serve the site at <http://localhost:1024>:

```sh
./bin/preview
```

This re-generates the site when it is modified, and restarts the
`cobalt` server when the `./_cobalt.yml` config file is modified (not
done by cobalt by default).

## How to publish

Build the site, outputting to `./docs`:

```sh
./bin/build
```

Use `git` to stage all changes, commit them, and push them to GitHub.

GitHub Pages will automatically deploy the new content.

## Links

Built with:

* [cobalt](https://cobalt-org.github.io/)
* [water.css](https://github.com/kognise/water.css)
