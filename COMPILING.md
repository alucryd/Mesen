To compile the Libretro core you will need a version of clang/gcc that supports C++14.
Run "make" from the "Libretro" subfolder to build the Libretro core.
LTO gives a large performance boost (25-30%+), so turning it off is not recommended.

To read ORE content (oxyromon's disc format) through libsmelt, add `ORE=1
SMELT_DIR=/path/to/oxyromon/crates/smelt-rs` to the make invocation; the
library must be built first with `cargo build --release` inside that folder.
Linux only for now.
