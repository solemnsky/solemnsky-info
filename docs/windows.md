# Developing on Windows

While on linux we can say "build the CMake project with the dependencies specified in our default.nix build expression" and expect things to work smoothly, on Windows this is not the case.

## MinGW distro

To make some of our gimmicky thirdparty dependencies work and avoid compatibility issues, I've opted to use a MinGW toolchain to build on Windows (instead of MSVC). Build using nuwen's maintained MinGW distro (http://nuwen.org/mingw.html) with no modifications. Use the latest release from the mentioned link -- if something doesn't work, post an issue on github please.

## CMake and IDE

solemnsky is built on the CMake build system. If your IDE doesn't support this, I'd recommend you use CLion. Set the CMake output path (File -> Settings -> Build, Execution, Deployment -> CMake -> Build output path) to ".\dist" to avoid some strange linking issues.

