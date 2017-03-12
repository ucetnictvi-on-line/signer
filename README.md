# Signer

This is a fork of original [Signer](https://badge.fury.io/rb/signer.svg) gem with applied patch for explicit signature namespaces.

## Why?

We needed the explicit namespaces feature for other gems and it's much easier to do so with normal ruby gem rather than github fork.

## Installation

```bash
gem install eet_signer
```

## Usage

For usage please see original gem's documentation. This gem should be rebased with the original gem at regularly.

### Explicit signature namespaces

If you need `Signature` tags to be in explicit namespace (say, `<ds:Signature>`) instead of to be in implicit default namespace you can specify next option:

```ruby
signer.ds_namespace_prefix = 'ds'
```
