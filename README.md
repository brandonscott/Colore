Colore
======

A powerful and elegant C# library for Razer Chroma's SDK

Contributing
------------

Contributors are very welcome! If you got code fixes, please [submit a pull request][newpull] here on GitHub.

If you want to join the development team, please contact [Sharparam][sharp] on GitHub.

All authors and contributors are listed in the **AUTHORS** file.

Please read the wiki page about [contributing][contrib] before submitting pull requests.

License
-------

Copyright &copy; 2015 by [Adam Hellberg][sharp] and [Brandon Scott][bs].

This project is licensed under the MIT license, please see the file **LICENSE** for more information.

Razer is a trademark and/or a registered trademark of Razer USA Ltd.  
All other trademarks are property of their respective owners.

This project is in no way endorsed, sponsored or approved by Razer.

Dependencies
------------

Colore depends on the Razer Chroma SDK (RzChromaSDK64.dll or RzChromaSDK.dll).

The Razer Chroma SDK is provided by Razer and [can be obtained from their website][rzdev].

Building
--------

It's important to note that this project doesn't build on the "AnyCPU" platform (which is the default
for C# projects). It builds against x86 to stay compliant with Razer's code which targets the x86
platform. When building with MSBuild, you'd run something like:

```
msbuild Colore.sln /p:Configuration=Release;Platform=x86
```

Make sure that your projects using Colore are also compiled against x86.

Colore does have a configuration mode that compiles it in AnyCPU, but it's untested, to run
that config, simply replace `Platform=x86` in the above command with `Platform=AnyCPU`.

Projects
--------

Current projects utilizing this or modified versions of this library:

*None right now!*

(If you want your project listed, just contact [Sharparam][sharp] or [Brandon][bs])

[newpull]: ../../pull/new/develop
[sharp]: https://github.com/Sharparam
[contrib]: ../../wiki/Contributing
[bs]: https://github.com/brandonscott
[rzdev]: http://developer.razerzone.com/chroma
