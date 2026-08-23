# Mercury, a fork of Pluto
Currently, you have to build Mercury

This will change.

### Prerequisites
* [MSYS2](https://msys2.org) if you're on Windows. You can use your preferred terminal if you're on Linux
  * In Windows the game must be built in the **UCRT64** or **MINGW64** shell, which come with MSYS2
  * Make sure when you have MSYS2 verify MINGW64 exists and open it. It should have a pinkish font like this
 <img width="162" height="39" alt="image" src="https://github.com/user-attachments/assets/661ca26a-ad0f-4931-b01c-6ab987300521" />
 
if you use UCRT itll be the same color but UCRT64
  
 <img width="140" height="49" alt="image" src="https://github.com/user-attachments/assets/63795069-0eb6-4fcf-9738-2724d0440ab5" />
 
 
  * Run `pacman -S gcc python binutils cjson git make mingw-w64-x86_64-glew`
  * A whole bunch of packages will install, please wait patiently

# 
  
### Compiling
You'll be using `git` and `make` commands, the builder will use the rest of those other packages you installed earlier

* Clone with the link of the repo: `git clone https://github.com/Kaiju2019/Mercury`
  * You can download the [source code](https://github.com/Kaiju2019/Mercury/archive/refs/heads/main.zip) if you prefer
    
* Run `cd Mercury` to get to the files or  `cd path\to\your\good\ol\build\folder`
  * (ex; `cd C:\Users\UrUserLol\Documents\game`) if you extracted the source code somewhere else
    
* Run `make` (or `make -j$(nproc)` to speed up compilation at the cost of using more CPU power)
  * The build will make your package manager (ex; pacman, on mingw64 by default) install necessary dependencies
    
* The built game will be located in the `build/us_pc` directory
  * On Windows, you can run `explorer build/us_pc` or `explorer .` if you're already in the build, to open File Explorer in that directory
    
To debug you can also `./sm64coopdx` on either os to see the log in real-time
