#whirlpool.go
a [whirlpool hashing](https://en.wikipedia.org/wiki/Whirlpool_(cryptography\)) library for go

## build status

[![Build Status](https://secure.travis-ci.org/jzelinskie/whirlpool.png)](http://travis-ci.org/jzelinskie/whirlpool)

## setup

```bash
$ go get github.com/jzelinskie/whirlpool
```

## example

```Go
package main

import (
  "fmt"
  "github.com/jzelinskie/whirlpool"
)

func main() {
  w := whirlpool.New()
  text := []byte("This is an example.")
  w.Write(text)
  fmt.Println(w.Sum(nil))
}
```

## docs

checkout the [gopkgdoc page](http://go.pkgdoc.org/github.com/jzelinskie/whirlpool), but there isn't much -- it works just like the other hashes in the standard library

## branches

* master - stable, works like the hash libs in the corelib
* trace - same code as master, but prints midstate values to stdout

## license

Modified BSD License
