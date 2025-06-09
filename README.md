# tflint-ruleset-terraform-sort

## Requirements

- TFLint v0.42+
- Go v1.24

## Installation

You can install the plugin with `tflint --init`. Declare a config in `.tflint.hcl` as follows:

```hcl
plugin "terraform-sort" {
  enabled = true

  version = "0.2.2"
  source  = "github.com/kenske/tflint-ruleset-terraform-sort"

}
```

## Rules

See [docs](docs) for a list of rules available in this ruleset.

## Building the plugin

Clone the repository locally and run the following command:

```
$ make
```

You can easily install the built plugin with the following:

```
$ make install
```

You can run the built plugin like the following:

```
$ cat << EOS > .tflint.hcl
plugin "template" {
  enabled = true
}
EOS
$ tflint
```
