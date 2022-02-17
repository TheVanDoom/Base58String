# Swift Base58String

Base58String is forked from this original [repository](https://github.com/cloutiertyler/Base58String) by Tyler Cloutier.

This repository reworks some aspects of the implementation and replaces deprecated functionality where possible.

## How to Install

### Swift Package Manager

Add the following to your Package.swift file in "dependencies".

```
.package(url: "https://github.com/cloutiertyler/Base58String.git", from: "1.0.0")
```

## Usage

```Swift
import Foundation
import Base58String

func test() {

    let data = Data([222, 100, 50])
    print("Data: \(Array(data))")

    let encoded = String(base58Encoding: data)
    print("Encoded string: \(encoded)")

    let decoded = Data(base58Decoding: encoded)!
    print("Decoded data: \(Array(decoded))")

}
```
