# go-wasm

## compile with go to wasm

```shell
GOOS=js GOARCH=wasm go build -o main.wasm main.go
```
--> 1974869 bytes

## compile with tinygo to wasm

```shell
tinygo build -target=wasm -no-debug -gc=leaking -opt=z -o main.wasm main.go
```
--> 91509 bytes

## compile with tinygo to wasm-wasi

```shell
tinygo build -wasm-abi=generic -target=wasi -no-debug -gc=leaking -opt=z -o main.wasm main.go
```
--> 136139 bytes

