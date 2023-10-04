# nix-httpx

Nix derivation for building the [httpx application](https://github.com/servicex-sh/httpx).

The httpx app is build as native binary using graalvm17-ce.

The binary is called `httpx-cli`.

Don't want to build it yourself? Use garnix cache:

```nix
{
  nix.settings = {
    substituters = [
      "https://cache.garnix.io"
    ];
    trusted-public-keys = [
      "cache.garnix.io:CTFPyKSLcx5RMJKfLo5EEPUObbA78b0YQ2DTCJXqr9g="
    ];
  };
}
```
