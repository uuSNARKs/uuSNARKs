# Benchmarking the Setup of Updatable zk-SNARKs

This code contains an implementation of the setup of 4 universal zk-SNARKs, which can be used for benchmarking and comparing the performance of the different schemes. 
The code is based on the [Arkworks](https://github.com/arkworks-rs) library.

The structure of this repository is as follows:
* basilisk_srs.rs: Rust code implementing the setup of Basilisk.
* lunarlite_srs.rs: Rust code implementing the setup of LunarLite.
* marlin_srs.rs: Rust code implementing the setup of Marlin.
* sonic_srs.rs: Rust code implementing the setup of Sonic.
* bin: directory containing scripts for benchmarking:
  - basilisk_timing.rs: Rust code for benchmarking Basilisk.
  - identifiable_security.rs: Rust code for benchmarking the algorithm for identifiable security (applied to Basilisk).
  - lunarlite_timing.rs: Rust code for benchmarking LunarLite.
  - marlin_timing.rs: Rust code for benchmarking Marlin.
  - sonic_timing.rs: Rust code for benchmarking Sonic.

## How to use
The only prerequisits are rust and cargo to be installed. 

To build the code, and get all necessary packages from [Arkworks](https://github.com/arkworks-rs):
```
cargo build
```

After this, you can run eg. basilisk_timing.rs:
```
cargo run --bin basilisk_timing
```
