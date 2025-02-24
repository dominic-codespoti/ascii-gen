# Rust ASCII Art Converter

This Rust tool converts images into ASCII art. It takes an image file as input, resizes it according to specified width and height parameters, and then converts the image into ASCII characters.

## Installation

Use cargo to quickly and easily install ascii-gen:

```bash
cargo install ascii-gen
```

## Usage

Run the tool:

```bash
ascii-gen path/to/your/image.jpg
```

Optional parameters:

- `--width`: Set the width of the output (default: 80)
- `--height`: Set the height of the output (default: 80)
- `--gamma`: Set the gamma of the ASCII art (default: 1.0)
- `--live`: Enable live editing of the ASCII art (default: false)

Examples:

```bash
ascii-gen path/to/your/image.jpg --width 120 --height 60
```

```bash
ascii-gen path/to/your/image.jpg --width 120 --height 60 --live
```

## Examples

### Input
![Input](./examples/duck.jpg "Input")

### Output (Small)
![Output](./examples/duck-ascii.png "Output")

### Output (Large)
![Output Large](./examples/duck-ascii-zoomed.png "Output Large")

## Dependencies

- [`clap`](https://docs.rs/clap/) - Command-line argument parser for Rust.
- [`image`](https://docs.rs/image/) - Image processing library for Rust.
- [`crossterm`](https://docs.rs/crossterm/) - Cross-platform terminal manipulation library for Rust.
- [`ratatui`](https://docs.rs/ratatui/) - TUI (Text-based User Interface) library for Rust.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Special thanks to the Rust community for their support and contributions.
