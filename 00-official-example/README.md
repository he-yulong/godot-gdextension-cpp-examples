# How to build offcial demo from scratch

```
cd extern/godot-cpp
scons platform=windows # generate bin/libgodot-cpp.windows.template_debug.x86_64.lib
cd ../../
```

```
cd 00-official-example
scons platform=windows
```

this will generate:
- `.dll` file
- `.lib` file (import library): Godot relies on `.gdextension` so it doesn't need this.
- `.exp` file: intermediate artifact. Godot doesn't need this.
