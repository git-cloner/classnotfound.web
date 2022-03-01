---
name: Introduction
---

# How do I implement classnotfound.com.cn



## Raising problems

  When developing Java applications, we often encounter ClassNotFoundException errors, which means that the specified class cannot be found, and sometimes NoClassDefFoundError errors occur. The reason is that the corresponding jar package is missing or the jar package is not placed in a directory recognized by the compiler. The reason for the problem is simple and easy to locate, but it is still difficult to find which jar is missing simply by class name. There is a foreign website findjar.com, which realizes the function of finding jar through class name, but this website may be due to the large number of visits, the website often can't open, and the access speed is very slow, so the idea of developing similar websites came into being.

After a period of development and data sorting, at present https://classnotfound.com.cn Online, source code in https://github.com/git-cloner/classnotfound Open source.