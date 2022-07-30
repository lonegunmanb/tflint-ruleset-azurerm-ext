# TFLint Ruleset for terraform-provider-azurerm-ext

TFLint ruleset extension plugin for Terraform Provider for Azure (Resource Manager)

## Requirements

- TFLint v0.35+
- Go v1.18

## Building the plugin

Clone the repository locally and run the following command:

```
$ make
```

You can easily install the built plugin with the following:

```
$ make install
```

To utilize the lastest Azure API info (this may cause incompatibility with current plugin version):

```
$ make updateSubmodule
$ make install
```

Note that if you install the plugin with make install, you must omit the `version` and `source` attributes in `.tflint.hcl`:

```hcl
plugin "azurerm-ext" {
    enabled = true
}
```

Follow the instructions to edit the generated files and open a new pull request.
