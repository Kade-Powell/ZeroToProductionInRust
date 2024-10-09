# Zero To Prod In Rust

## CI steps for later

```bash
###In our CI pipeline we would like to fail the linter check if clippy emits any warnings. We can achieve it with
cargo clippy -- -D warnings
###In our CI pipeline we will add a formatting step
cargo fmt -- --check”
### Security audit
cargo audit
```

## Install faster linker if you want

since this issue is close to resolved and active on nightly rust this project wont use it

- <https://github.com/rust-lang/rust/issues/39915#issuecomment-2116969891>
  - If work is not completed -> brew install llvm
    - follow the steps in -> brew info llvm

## cargo tools you need installed

- cargo watch
  - <https://github.com/watchexec/cargo-watch>
- cargo cargo llvm-cov
  - <https://github.com/taiki-e/cargo-llvm-cov>
- cargo cargo-audit
  - <https://github.com/RustSec/rustsec/tree/main/cargo-audit>
