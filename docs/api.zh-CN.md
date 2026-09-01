# API 参考

[English](api.md) | [文档索引](README.zh-CN.md)

本清单由本仓库 package 的 `go doc -short` 生成，用于快速查看公共面。精确语义以源码和测试为准。

## 包

### `gnalloy.org/codec-stomp`

包名：`stomp`

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
