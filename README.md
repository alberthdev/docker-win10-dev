# Windows 10 Development Environment Docker Image

This Docker image contains a rough set of packages installed to get you started quickly with development.

This image includes Windows 10 20H2 as the base, Chocolatey as another layer for package installation, and the following Chocolatey packages:

 * git
 * cmake
 * kb2999226
 * visualstudio2019buildtools
 * visualstudio2019-workload-vctools
 * powershell-core
 * vcredist-all

In addition, it installs the latest vcpkg to C:\vcpkg for use in your projects.

## Getting Started
Build the environment by running:

    docker build -t win10-dev .

To start the container with your environment + Powershell running, use:

    docker run --name win10-dev-ct -it win10-dev pwsh

