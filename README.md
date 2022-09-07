# economics-book

## Requirements

- Docker (latest version)
- Docker Compose (latest version)

## Execute

### Python Environment

```sh
docker compose up
```

- Build Book
    - See [documents](https://jupyterbook.org/en/stable/start/build.html).

```sh
jupyter-book create book
jupyter-book build book
```

- Publish Book
    - This command does create branch `gh-pages` automatically, and `git push origin gh-pages`. You should **NOT** `push` to this branch.
    - See [documents](https://jupyterbook.org/en/stable/start/publish.html).

```sh
ghp-import -n -p　-f book/_build/html
```
