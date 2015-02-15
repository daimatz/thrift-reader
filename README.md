# thrift-reader

Simple Thrift Struct Reader

## Instllation

```sh
bundle install --path vendor/bundler
rake DIR=/path/to/thrift/dir
```

## Usage

```sh
# read Thrift binary from stdin
cat /path/to/thrift/binary/file | bundle exec ./reader --format binary --struct StructName --pretty

# read Thrift binary from local file
bundle exec ./reader --format binary --struct StructName --input /path/to/thrift/binary/file --pretty

# read Thrift JSON from stdin
cat /path/to/thrift/json/file | bundle exec ./reader --format json --struct StructName --pretty

# read Thrift JSON from local file
bundle exec ./reader --format json --struct StructName --input /path/to/thrift/json/file --pretty
```
