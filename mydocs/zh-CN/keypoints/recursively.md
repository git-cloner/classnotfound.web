---
name: 递归获取jar包路径
---

# 递归获取jar包路径

对于https://repo1.maven.org/maven2/ 这个的逐级且深度不定的目录结构，获取最后一级jar的方法是要用到递归的，但由于递归越深，需要的栈空间越大，性能越差，所以在具体实现中，是将前三级目录先用循环方式存储下来，然后以第三级目录（如 https://repo1.maven.org/maven2/abbot/costello/ ）为基础，递归查找jar，且忽略掉test、javadoc之类的辅助jar，这样需要下载的jar的个数就会大大降低。