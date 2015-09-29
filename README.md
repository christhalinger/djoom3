#djoom3 - a Doom 3 Java port.

####05-02-15:
-Initial non playable release.

![http://wiki.djoom3.googlecode.com/git/init_menus.png](http://wiki.djoom3.googlecode.com/git/init_menus.png)

![http://wiki.djoom3.googlecode.com/git/title.png](http://wiki.djoom3.googlecode.com/git/title.png)




----------

#README.md#

####Enable OpenAL
Add/edit the following settings to the **DoomConfig.cfg** file:

- seta s_useOpenAL "1"
- seta s_libOpenAL "openal.dylib"

####How to build:
TODO

####How to run in an IDE:
#####IntelliJ
1. [https://www.jetbrains.com/idea/help/opening-reopening-and-closing-projects.html](https://www.jetbrains.com/idea/help/opening-reopening-and-closing-projects.html)
2. [Create a run configuration](https://www.jetbrains.com/idea/help/creating-and-editing-run-debug-configurations.html) for **neo.sys.win_main.java** 
3. Add **-Djava.library.path=/bla/natives**(location of the lwjgl native dll/so files) to the VM parameters of the [run configuration] (https://www.jetbrains.com/idea/help/setting-configuration-options.html)
4. Add **"+set fs_basepath '~/.local/share/Steam/steamapps/common/doom 3' +set com_allowConsole 1 +set si_pure 0"**(with quotes) to the program arguments of the [run configuration] (https://www.jetbrains.com/idea/help/setting-configuration-options.html)

###Important
####Operator Overloading:####
|c++|java|
|---------|------------|
|operator=| oSet(value)|
|operator[]| oSet(x, value)|
|operator[]|oGet(x)|
|operator[][]| oGet(x, y)|
|operator[][]| oSet(x, y, value)|
|operator+| oPlus|
|operator-| oMinus|
|operator*| oMultiply|
|operator/| oDivide|
|operator-()| oNegative|
|operator+=| oPluSet|
|operator-=| oMinSet|
|operator*=| oMulSet|
|operator/=| oDivSet|