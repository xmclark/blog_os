# the blog os

This is made following the [phil-opp OS tutorial](https://os.phil-opp.com/).

## how to do a build

You need to install lots of stuff.

Set the nightly compiler:

`> rustup override set (insert_nightly_triple)`

Add the rust source component:

`rustup component add rust-src`

Add the special LLVM tools component:

`rustup component add llvm-tools-preview`

Install xbuild:

`cargo install cargo-xbuild`

Install bootimage:

`cargo install bootimage --version "^0.7.3"`

Install QEMU:

https://www.qemu.org/download/

**And finally, to run the emulator:**

`cargo xrun`