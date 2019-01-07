# View Annotated File

<img src="/Inspector_Gadget.png" data-canonical-src="/Inspector_Gadget.png" width="200" height="400" />

## Install

```
go get github.com/ValeryPiashchynski/inspector-gadget
```

## Usage go1.9

```
go build -a -gcflags "-m -m -d=ssa/check_bce/debug" project 2> analysis.log
inspector-gadget analysis.log
```

## Usage go1.10

```
go build -a -gcflags "all=-m -m -d=ssa/check_bce/debug" project 2> analysis.log
inspector-gadget analysis.log
```
