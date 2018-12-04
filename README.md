# [go-mnemonic][mnemonic]: cryptographic entropy mnemonics

[![IPFN project][badge-ipfn]][org-ipfn]
[![IPFN Documentation][badge-docs]][docs]
[![See COPYING.txt][badge-copying]][COPYING]
[![GoDoc][badge-godoc]][godoc-ipfn]
[![Travis CI][badge-ci]][ci]
[![Coverage Status][coverage-badge]][coverage-status]

Go implementation of the mnemonic seeds as defined in [bip39][].

## Usage

```go
package main

import (
  "fmt"

  "github.com/ipfn/go-mnemonic/mnemonic"
)

func main(){
  entropy, _ := mnemonic.NewEntropy(256)
  mnemonic, _ := mnemonic.New(entropy)

  fmt.Printf("Entropy: %x\n", entropy)
  fmt.Printf("Mnemonic: %s\n", mnemonic)
}
```

## License

See [COPYING][COPYING] file for licensing details.

## Credits

Source code was forked from [tyler-smith/go-bip39](https://github.com/ipfn/go-mnemonic).

Wordlists are from the [bip39][].

Test vectors are from the standard Python BIP0039 implementation from the
Trezor team: [https://github.com/trezor/python-mnemonic](https://github.com/trezor/python-mnemonic)

## Project

This source code is part of [IPFN](https://github.com/ipfn) – interplanetary functions project.

[ci]: https://travis-ci.org/ipfn/go-mnemonic
[docs]: https://docs.ipfn.io/
[COPYING]: https://github.com/ipfn/go-mnemonic/blob/master/COPYING
[badge-ci]: https://travis-ci.org/ipfn/go-mnemonic.svg?branch=master
[badge-copying]: https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square
[badge-docs]: https://img.shields.io/badge/documentation-IPFN-blue.svg?style=flat-square
[badge-godoc]: https://godoc.org/github.com/ipfn/go-mnemonic/mnemonic?status.svg
[badge-ipfn]: https://img.shields.io/badge/project-IPFN-blue.svg?style=flat-square
[coverage-badge]: https://coveralls.io/repos/github/ipfn/go-mnemonic/badge.svg?branch=master
[coverage-status]: https://coveralls.io/github/ipfn/go-mnemonic?branch=master
[org-ipfn]: https://github.com/ipfn
[godoc-ipfn]: https://godoc.org/github.com/ipfn/go-mnemonic/mnemonic
[mnemonic]: https://github.com/ipfn/go-mnemonic/
[bip39]: https://github.com/bitcoin/bips/tree/master/bip-0039