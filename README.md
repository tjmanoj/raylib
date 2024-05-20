# Setting up vcpkg and Installing raylib

This guide will help you set up vcpkg, a C++ library manager, and use it to install the raylib library.

## Steps

1. **Clone the vcpkg Repository**

    First, clone the vcpkg repository from GitHub:
    ```sh
    git clone https://github.com/microsoft/vcpkg.git
    ```

2. **Rename the Folder**

    Rename the `vcpkg-master` folder to `vcpkg`:
    ```sh
    mv vcpkg-master vcpkg
    ```

3. **Open PowerShell and Navigate to the vcpkg Folder**

    Open PowerShell and navigate to the `vcpkg` folder:
    ```sh
    cd path\to\vcpkg
    ```

4. **Bootstrap vcpkg**

    Run the bootstrap script to build vcpkg:
    ```sh
    ./bootstrap-vcpkg.bat
    ```

5. **Integrate vcpkg with Your System**

    Integrate vcpkg with your system so you can use it from any command prompt:
    ```sh
    ./vcpkg integrate install
    ```

6. **Install raylib**

    Use vcpkg to install the raylib library for x64 Windows:
    ```sh
    ./vcpkg install raylib:x64-windows
    ```

7. **Import raylib in Your Project**

    In your C++ project, include the raylib header:
    ```cpp
    #include "raylib.h"
    ```

## Additional Information

- For more information on vcpkg, visit the [official GitHub repository](https://github.com/microsoft/vcpkg).
- Detailed documentation for raylib can be found on the [raylib website](https://www.raylib.com/).

With these steps, you should have vcpkg set up and raylib installed and ready to use in your C++ projects.
