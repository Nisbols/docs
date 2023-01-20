# Environment setup
## Tools
- WASM-4
- WASI-SDK
- PowerShell
- Windows Terminal

> **_NOTE:_** C needs to be setup first

## Steps
1. Download and install [WASM-4](https://wasm4.org/)
2. Download and install [WASI-SDK](https://github.com/WebAssembly/wasi-sdk)
3. Set environment parameters for WASI-SDK using powershell

```PS
$INCLUDE = "C:\wasi-sdk-16.0\bin"

[Environment]::SetEnvironmentVariable("WASI_SDK_PATH", "$INCLUDE, "Machine")

```

You can now use use WASM-4.