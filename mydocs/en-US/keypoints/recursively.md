---
name: Get jar package path recursively
---

# Get jar package path recursively

For the hierarchical and indeterminate directory structure of https://repo1.maven.org/maven2/ , the method of obtaining the last level of jars requires recursion, but the deeper the recursion, the larger the stack space required , the worse the performance, so in the specific implementation, the first three-level directory is stored in a circular manner, and then the third-level directory (such as https://repo1.maven.org/maven2/abbot/costello/ ) is used as Basically, recursively search for jars, and ignore auxiliary jars such as test and javadoc, so that the number of jars to be downloaded will be greatly reduced.