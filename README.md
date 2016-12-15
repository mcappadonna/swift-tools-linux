# swift-tools-linux
This repository contain a list of scripts and tools I've wrote in order to make developing Swift code on Linux more productive (for me).
Here a list of the available tools and functionalities:

## swift-continuous-build
This simple bash script will work from a Swift executable project directory. You can initialize the directory with the swift command:

    $ swift project init --type executable

Into that directory, you can launch the script to constantly checking your source files and recompile the project when something changes.
Simply copy the scripts in a directory available in your $PATH and launch it from your project root directory:

    $ swift-continuous-build

If you need to pass some parameters to your compiled binary, just pass those as parameters to swift-continuous-build script, they will be forwarded to your compiled software.
