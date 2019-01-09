UWindsor COMP-3520 SDL2 Project Template (CMake version)
===

This template is intended for students in the COMP-3520 Introduction to Computer Graphics course
at the University of Windsor, however it should serve as a useful template for anyone interested in
getting started with the [SDL2](http://libsdl.org/) library quickly on non-Windows platforms.

The following dependencies are required:
* [CMake](https://cmake.org/)
* [SDL2](http://libsdl.org/) 
* [SDL2_ttf](https://www.libsdl.org/projects/SDL_ttf/) library for easy text rendering
* [freetype2](https://www.freetype.org/) which `SDL2_ttf` uses for the actual work

It's very easy to get started with SDL2 on most linux distributions.  Just ensure you have the above packages installed along with their header files (usually requires a `-dev` package)

On Debian based systems, the packages will probably be called `libsdl2-dev` and `libsdl2-ttf-dev`.
On Arch Linux, look for the packages `sdl2` and `sdl2_ttf`.

Mac users should be able to use Homebrew or a similar package manager to install the needed dependencies.
If you need help, just send me an email.

Setup
---

Once you've installed these packages, you'll be all set to start your first assignment.
Clone this repository somewhere using Git (in a shell):

~~~
git clone https://github.com/InBetweenNames/SDL2TemplateCMake.git
cd SDL2TemplateCMake
~~~

Next, enter the build directory:

~~~
cd build
~~~

Run CMake:

~~~
cmake ..
~~~

If this runs without errors, you're ready to build:

~~~
cmake --build .
~~~

Now, run the demo:

~~~
./main
~~~

Note that `iosevka-regular.ttf` must be in the working directory of `main` for it to work.
In practice, this means you need to be in the `build` directory when running `main`.
I would welcome a pull request that removes this restriction.

The demo
---

The sample code provided should display "Hello World!" in a window on your screen when run.
You can clone this project as many times as you need for different assignments.

Recommended practices
---

Students who know C++ are encouraged to use it, however, C++ is not a requirement for the course.
The sample code provided is mostly C compatible for the benefit of students who haven't had much C++ exposure yet.

When we get to the more mathy parts of the course, if you have a good handle on C++, consider using
[Eigen](http://eigen.tuxfamily.org/index.php?title=Main_Page) for your Linear Algebra needs.

Extra goodies:
---

Although this template has everything you need to succeed in the course, in your own personal projects
it's likely you'll want to go even further.  Consider adding the following libraries for your arsenal:

* [SDL2_image](https://www.libsdl.org/projects/SDL_image/) for easy image loading from a variety of formats
* [SDL2_net](https://www.libsdl.org/projects/SDL_net/) for a basic cross-platform networking library
* [SDL2_mixer](https://www.libsdl.org/projects/SDL_mixer/) for sound rendering
* [SDL2_rtf](https://www.libsdl.org/projects/SDL_rtf/) for basic document handling (RTF)

Bugs:
---

If you find any problems with the template, please let me know by either creating an Issue on the project page or sending
me an email.
