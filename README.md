# lern-dotnet
lerning dotnet framework

## download 

```
https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/sdk-7.0.302-linux-x64-binaries
```

### dotnet-sdk-7.0.302-linux-x64.tar.gz

## create file 

```sh
DOTNET_FILE=dotnet-sdk-7.0.302-linux-x64.tar.gz
export DOTNET_ROOT=$(pwd)/.dotnet
mkdir -p "$DOTNET_ROOT" && tar zxf "$DOTNET_FILE" -C "$DOTNET_ROOT"
export PATH=$PATH:$DOTNET_ROOT:$DOTNET_ROOT/tools
```

### nano loaddot.sh

### sudo chmod +x loaddot.sh

### ./loaddot.sh

## set the following two environment variables in your shell profile

nano .bashrc

```sh
export DOTNET_ROOT=$HOME/.dotnet
export PATH=$PATH:$HOME/.dotnet:$HOME/.dotnet/tools
```

## check command

```sh
dotnet --list-sdks
dotnet --list-runtimes
```

## example project 

```sh
mkdir test-dot
cd test-dot/
dotnet new console --framework net7.0
```

### nano Program.cs

```
Console.WriteLine("Hello, World!");
```

## run 

```sh
dotnet run
```

### Or

```sh
cd test-dot/bin/Debug/net7.0
./test-dot
```


