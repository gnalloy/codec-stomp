# API Reference

[简体中文](api.zh-CN.md) | [Docs Index](README.md)

This inventory is generated from `go doc -short` for the packages in this repository. It is a quick public-surface map; source files and tests remain the authority for exact semantics.

## Packages

### `gnalloy.org/codec-stomp`

Package name: `stomp`

```text
var ErrInvalidFrame = errors.New("gnalloy/codec/stomp: invalid frame") ...
type Command string
    const CommandConnect Command = "CONNECT" ...
type Decoder struct{ ... }
    func NewDecoder(maxHeaderBytes int, maxBodyBytes int) (*Decoder, error)
type Encoder struct{}
    func NewEncoder() *Encoder
type Frame struct{ ... }
    func Heartbeat() Frame
    func NewFrame(command Command, headers Headers, body buffer.ByteBuf) Frame
type Header struct{ ... }
type Headers []Header
```
