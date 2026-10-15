# Mobile Linux on Android: Architecture Notes

## Reference stack

```text
Desktop application / shell
            |
     Display protocol
      (X11 / Wayland)
            |
       Display server
  (for example, Termux:X11)
            |
  Graphics libraries / drivers
   (Mesa, device-dependent)
            |
      Termux userspace
            |
      Android kernel
            |
       ARM64 hardware
```

This is a conceptual model, not a guarantee that every component works on every device. The actual stack depends on the application, Termux packages, Android version, GPU driver availability, and display-server configuration.

## Key distinctions

- **Native Termux userspace:** programs are built for and run in Termux's environment.
- **Proot distribution:** a Linux distribution filesystem and userland are provided through a user-space compatibility layer; this is not the same as booting a separate Linux kernel.
- **X11:** a display protocol used by many desktop applications.
- **Wayland:** a display protocol with a different compositor/client model.
- **Mesa:** a collection of graphics libraries and drivers; hardware support varies by GPU and Android environment.
- **LLVMpipe:** a CPU-based software rasterizer that can provide compatibility but may be slow.

## Record what was actually used

For each experiment, write down whether the session used native Termux packages, a proot distribution, X11 or Wayland, hardware acceleration or software rendering, and the exact versions. Avoid claiming GPU acceleration solely because a desktop window appeared.
