Welcome to the meson quick guide!
__________________________________
Description:
While the Wiki is very helpful, it can be lacking at times and that is where this comes in.
__________________________________
Meson has two main dependencies
* Python 3
* Ninja
(From here on out, most work will be done in the terminal).

sudo apt install python3 ninja-build
__________________________________
Compiling:
cd /home/vm/Projects/hello_world (this navigates or changes directory to the file location specified).

mkdir build (here we make a new directory or folder to put the files soon to be generated).
cd build (navigate into the build directory).
meson .. (this tells meson to put the build contents in the build directory using the files outside the directory).
ninja (invokes the fast ninja build system to complete setup).
ninja hello_world
__________________________________
Tip: 
To recompile just invoke ninja again by typing
ninja

If you want optimized binaries just add the following
--buildtype=debugoptimized

You'll want to keep each type of build separate so create a new directory like before
mkdir optimized_build (this is not necessary unless you plan to use optimized builds).

