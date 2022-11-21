# OpenGL

This is a simple OpenGL project that I made to learn OpenGL.

## Environment

```yaml
# Windows 10 x64

# Visual Studio 2019
- Change Project Setings
  # project -> Properties -> General
  - input directory: $(SolutionDir)bin\$(Platform)\$(Configuration)\
  - intermediate directory: $(SolutionDir)bin\intermediates\$(Platform)\$(Configuration)\
  # project -> Properties -> C/C++ -> General
  - Additional Include Directories: [
      $(SolutionDir)Dependencies\GLFW\include\
      $(SolutionDir)Dependencies\GLEW\include\
    ]
  # project -> Properties -> C/C++ -> Preprocessor
  - Preprocessor Definitions: [
      GLEW_STATIC
      _MBCS
      %(PreprocessorDefinitions)
    ]
  # project -> Properties -> Linker -> General
  - Additional Library Directories: [
      $(SolutionDir)Dependencies\GLFW\lib-vc2019\
    ]
  # project -> Properties -> Linker -> Input
  - Additional Dependencies: glew32s.lib;glfw3.lib;opengl32.lib;User32.lib;Gdi32.lib;Shell32.lib;
```

## External Libraries

- [GLFW](https://www.glfw.org/)
- [GLEW](https://glew.sourceforge.net/)

## Thanks

- TheCherno
