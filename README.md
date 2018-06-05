# Golang Setup on Ubuntu

## Installing Go

#### Prerequisites

Emacs/Vim

### Installing Go on Ubuntu

```
sudo apt install golang-go
```

Check cache for golang

```
apt-cache show golang | less
```

### Setup PATH

```
export GOPATH=/home/ubuntu/workspace/go
```
#### Retrieve GOPATH

```
echo $GOPATH
```

```
export PATH=$PATH:$GOPATH/bin
```

### Create Hello World Program using this repo as a domain

```
mkdir $GOPATH/src/marouaneabra.github.io/Go/helloworld/ -p
emacs $GOPATH/src/marouaneabra.github.io/Go/helloworld/hello.go
```

### Compile Go Program

```
go install marouaneabra.github.io/Go/helloworld
```

### Run Hello World Program

```
helloworld
```