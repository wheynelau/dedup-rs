# dedup-rs

Rust implementation of deduplication algorithms with Python bindings.

**Note:** This repository is used in conjunction with [text-dedup-rs](https://github.com/wheynelau/text-dedup-rs):
- [dedup-rs](https://github.com/wheynelau/dedup-rs) - Rust implementation (this repo)
- [text-dedup-rs](https://github.com/wheynelau/text-dedup-rs) - Python package that uses dedup-rs

## Components

This workspace contains three crates:

- **dedup-core**: Core deduplication algorithms and data structures
- **dedup-bin**: Command-line interface for deduplication
- **dedup-py**: Python bindings via PyO3

## Building

```bash
cargo build --release
```

## Testing

```bash
cargo test
```

## Python Bindings

The `dedup-py` crate provides Python bindings using PyO3. The Python package can be installed via pip (wheels are built automatically via CI).

### For Developers

To build the Python bindings locally during development:

```bash
pip install maturin
maturin develop
```

## License

Apache License 2.0
