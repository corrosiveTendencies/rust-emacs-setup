# rust-emacs-setup
Rust Emacs IDE set-up based on / stolen from http://manenko.com/2016/08/03/setup-emacs-for-rust-development.html

# .bash_profile setup
You need to declare RACER_CMD and RUST_SRC_PATH for Emacs

PATH=$PATH:$HOME/.local/bin:$HOME/bin

export PATH
export CARGO_INCREMENTAL=1
export PATH="$HOME/.cargo/bin:$PATH"
export RACER_CMD="$HOME/.cargo/bin/racer"
export RUST_SRC_PATH="$(rustc --print sysroot)/lib/rustlib/src/rust/src"

