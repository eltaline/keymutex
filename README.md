# keymutex
A golang key set mutex

## Example
```go
var kmutex = keymutex.New(47)

// ...
go func(key string) {
    kmutex.Lock()
    defer kmutex.Unlock()
    // do something with the key
}(akey)
```
