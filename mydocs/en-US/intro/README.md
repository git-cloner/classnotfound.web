---
name: Introduction
---

# classnotfound.com.cn



## Solution

When developing Java applications, it is common to encounter ClassNotFoundException errors, which mean that the specified class cannot be found, and sometimes There will be NoClassDefFoundError errors, which are due to the lack of the corresponding jar package, or the jar package is not placed in a directory recognized by the compiler. The reason for the problem is simple and easy to locate, but it is still difficult to find out which jar is missing simply by the class name. There is a foreign website findjar.com, which implements the function of finding jars through class names, but this website may be due to the large number of visits, the website is often not opened, and the access speed is very slow, so the idea of developing similar websites has been generated.

After a period of development and data collation work, the https://classnotfound.com.cn has been launched, and the source code has been open sourced https://github.com/git-cloner/classnotfound.

https://classnotfound.com.cn Implement the ability to search for jars by class name and jar package name if the keyword is determined by "." Separated, it is considered to be the class name, otherwise it is the jar package name, and the retrieved jar package can view the historical version and the POM file at the same time.