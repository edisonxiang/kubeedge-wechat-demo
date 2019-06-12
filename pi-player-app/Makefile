.PHONY: all build pi-player-app clean

all:build

build:pi-player-app

pi-player-app:
	export GOARCH=arm
	export GOOS="linux"
	export GOARM=6
	export CGO_ENABLED=1
	export CC=arm-linux-gnueabi-gcc
	go build -o pi-player-app main.go

clean:
	rm -rf ./pi-player-app
