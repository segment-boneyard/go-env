
# go-env

 [![Build Status](https://travis-ci.org/segmentio/go-env.svg?branch=master)](https://travis-ci.org/segmentio/go-env)

 Tiny wrapper around getenv() to return an error instead of an empty string when missing.

## Usage

#### func  Get

```go
func Get(name string) (string, error)
```
Get env var `name` or return an error if it's missing.

#### func  GetDefault

```go
func GetDefault(name string, value string) string
```
GetDefault returns `value` if environment variable `name` is not present.

#### func  MustGet

```go
func MustGet(name string) string
```
MustGet panics if the environment variable is missing.


# License

 MIT