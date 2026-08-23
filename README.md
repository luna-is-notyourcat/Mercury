# Mercury
(a fork of Pluto)

## Download

Prebuilt executables for Windows and Linux of Pluto can be downloaded from the [releases](https://github.com/Llennpie/Pluto/releases/latest) page

## Building

### Prerequisities

* [MSYS2](https://msys2.org) if you're on Windows
  * Pluto must be built in the **UCRT64** or **MINGW64** shell
  * The built-in updater will be disabled for MINGW64 builds
  * Make sure when you have MSYS2 verify MINGW64 exists and open it. It should have a pinkish font like this
  <img width="162" height="39" alt="image" src="https://github.com/user-attachments/assets/661ca26a-ad0f-4931-b01c-6ab987300521" />
  
### Compiling
You'll be using `git` and `make` commands 
* Clone the repository using git: `git clone https://github.com/Llennpie/Pluto`
  * Alternatively you can [download the source code](https://github.com/Llennpie/Pluto/archive/refs/heads/main.zip)
  * Once this is done, you may extract the archive to any preferred folder, but make sure to `cd path/to/your/pluto` rather than just cd Pluto (Your file wont be found that easily unless you put it in here (C:/YOUR USER!!!/msys64/home)
<img width="297" height="37" alt="image" src="https://github.com/user-attachments/assets/b38b0388-1d98-4b33-86e7-e7e302c8801d" />
* Run `cd Pluto` to enter the Pluto source tree
* Run `make` (or `make -j$(nproc)` to speed up compilation at the cost of using more CPU power)
  * This also invokes your package manager to install necessary dependencies
* The built game will be located in the `build/us_pc` directory
  * On Windows, you can use the `explorer build/us_pc` to open File Explorer in that directory
