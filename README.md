INTRODUCTION:
-------------
This is a module for the Wonkey programming language that allows you to save/load data to your browser's localStorage using a Stream object. It is mainly
intended to write local save files for your browser games.

INSTALLATION:
-------------
Copy the localstoragestream folder into the modules folder of your Wonkey installation. Build the module using `wake -mods -target=emscripten`

USAGE:
------
Once installed, you can import the module by adding `#Import "<localstoragestream>"` and `Using luc.localstoragestream` to the beginning of your code. Note that
if your project is multi-target, both of these should be enclosed by `#If __WEB_TARGET__` blocks. You can then use `Stream.Open("localstorage::[...]` to create
a Stream object that you can use in the same way as other Stream objects.
For a usage example, take a look at localstoragetest.wx.
