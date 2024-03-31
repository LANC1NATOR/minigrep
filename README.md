# minigrep

**minigrep** is a simple command-line utility written in Rust that searches for a query string in a specified file. It offers basic functionality to search for a given query, with an option to perform a case-insensitive search.

## Usage

To use **minigrep**, run the following command:

```bash
minigrep <query> <file_path>
```

- `<query>`: The string you want to search for.
- `<file_path>`: The path to the file in which you want to search.

By default, **minigrep** performs a case-sensitive search. To enable case-insensitive search, set the `IGNORE_CASE` environment variable:

```bash
export IGNORE_CASE=1
minigrep <query> <file_path>
```

## Example

```bash
minigrep duct poem.txt
```

This will search for the string "duct" in the file `poem.txt` and display the lines containing the match.

## Installation

To build and install **minigrep**, you need to have Rust installed. If you haven't installed Rust, you can do so using [rustup](https://rustup.rs/).

Once you have Rust installed, you can build **minigrep** using Cargo:

```bash
git clone https://github.com/yourusername/minigrep.git
cd minigrep
cargo build --release
```

This will create the executable `minigrep` in the `target/release/` directory. You can then copy this executable to a directory in your `PATH` to make it accessible from anywhere.

## Tests

**minigrep** includes unit tests to ensure its functionality. To run the tests, use Cargo:

```bash
cargo test
```

This will execute the test suite and ensure that all the functions are working as expected.

---

Feel free to contribute, report issues, or suggest improvements!