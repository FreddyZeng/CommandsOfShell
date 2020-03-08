# CommandsOfShell

## xcrun

Print Mac-0 file swift function to origin function symbol (swift-demangle)

```shell
xcrun nm -nm <Mac-O file path> | grep -oe "\$.*" | egrep -oe '\$[a-zA-Z0-9_]+\b' | tr -d "$" | xargs xcrun swift-demangle {}
```