# Examples

This folder contains example scripts that can be used to interact with
the `aws-secrets` crate.

## Quickstart

[cargo-rx]: https://github.com/rnag/cargo-rx

Install my crate [cargo-rx], which abstracts away `cargo run --example`.
This provides a single `rx` command.

```shell
❯❯ cargo install cargo-rx
```

Now start out by cloning the GitHub project:

```shell
❯❯ git clone https://github.com/rnag/aws-secrets.git
```

Then, simply `cd` into the project folder:

```shell
❯❯ cd aws-secrets
```

From here, you can use `rx` to build and run
any of the examples individually.

In particular, here's a sample usage of running `examples/demo.rs`:

```shell
❯❯ rx demo
```

If you run the command without any arguments, you can select 
from the list of available examples:

```shell
❯❯ rx
```

To pass arguments to a script, you can include them after the `--`.

For instance, here's an example of passing arguments to the `sm_show_secret` script:

```shell
❯❯ rx sm_show_secret -- -s "My Secret"
```