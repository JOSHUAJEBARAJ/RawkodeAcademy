# Content Management

## Linter

The file linter resides in [linter](linter). When a file is valid, it exits with a status code of 0. When a file is invalid, it exits with a status code of 1 and prints the errors to standard error.

Supported file formats (links to their respective directories including examples):

* [Episodes](data/episodes/)
* [People](data/people/)
* [Shows](data/shows/)
* [Technologies](data/technologies/)

### Usage

To run the linter, use the following command:

```shell
cargo run --manifest-path=linter/Cargo.toml -- lint --path data/episodes/
```

To format all files, use the following command:

```shell
cargo run --manifest-path=linter/Cargo.toml -- format --path data/ [--apply]
```
