# Ratatui template

This repo is entirely based off of Chris Titus' [linutil](https://github.com/ChrisTitusTech/linutil).

The `linutil` program was entirely stripped from the TUI, leaving only a template for quickly spinning up new projects using Ratatui (🦀).

## Usage

There are a few files which contained a reference to the `linutil` project. Since this is a template, those entries have all been replaced with placeholders.

It is highly suggested that any first commit should be to correct the placeholders.

The following is a list of the different placeholder values:

- `PLACEHOLDER_TITLE`
    - This should be the formatted, capitalized name of the project.
    - Using the `linutil` project as an example, this value would be `Linutil`.
- `PLACEHOLDER_NAME`
    - This should be the unformatted, uncapitalized name of the project.
    - Using the `linutil` project as an example, this value would be `linutil`.

The following is a list of all files with the placeholders:

- `LICENSE`
    - Line 3 - regarding user's name.
- `core/Cargo.toml`
    - Change all instances of placeholders.
    - In addition, review the value for `repository`.
- `core/src/inner.rs`
    - Change `PLACEHOLDER_NAME`.
- `man/PLACEHOLDER_NAME.1`
    - This file should be renamed, and all instances with placeholders should be replaced.
        - Note that this file has additional values to change, including:
            - Line 2 - publication dates.
            - Line 11 - the description of the project (`DESCRIPTION`).
            - Lines 45, 45, 56 - regarding user's name.
- `tui/Cargo.toml`
    - Change all instances of placeholders.
    - In addition, review the value for `documentation` and `repository`.
- `tui/src/confirmation.rs`
    - Change `PLACEHOLDER_NAME`.
- `tui/src/filter.rs`
    - Change `PLACEHOLDER_NAME`.
- `tui/src/floating_text.rs`
    - Change `PLACEHOLDER_NAME`.
- `tui/src/running_command.rs`
    - Change `PLACEHOLDER_NAME`.
- `tui/src/state.rs`
    - Change all instances of placeholders.
    - Lines 309, 310 - Split `PLACEHOLDER_TITLE` so the first part is **bold** and the second is *italic*.
- `xtask/Cargo.toml`
    - Change `PLACEHOLDER_NAME`.
- `xtask/src/docgen.rs`
    - Change `PLACEHOLDER_NAME`.

The best way to achieve this is to do a "find-and-replace" across multiple files to replace `PLACEHOLDER_TITLE` and `PLACEHOLDER_NAME`. Then, address the more specific changes to:

- `LICENSE`
- `core/Cargo.toml`
- `man/PLACEHOLDER_NAME.1`
- `tui/Cargo.toml`
- `tui/src/state.rs`
