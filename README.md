# version-cutting-ghaction

#### Using the `packer init` command
Starting from version 1.7, Packer supports a new `packer init` command allowing
automatic installation of Packer plugins. Read the
[Packer documentation](https://www.packer.io/docs/commands/init) for more information.
To install this plugin, copy and paste this code into your Packer configuration .
Then, run [`packer init`](https://www.packer.io/docs/commands/init).
```hcl
packer {
  required_plugins {
    amazon = {
      version = ">= 2.0.6"
      source  = "github.com/hashicorp/amazon"
    }
  }
}
```
