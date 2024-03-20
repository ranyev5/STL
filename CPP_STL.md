# **STL 源码解析**

## 依赖

### 本地测试环境版本 

``` shell
$ g++ --version
g++ (Ubuntu 11.4.0-1ubuntu1~22.04) 11.4.0
Copyright (C) 2021 Free Software Foundation, Inc.
This is free software; see the source for copying conditions.  There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
```

### STL源码下载

``` shell
$ git clone https://github.com/gcc-mirror/gcc.git
$ cd gcc && git checkout releases/gcc-11.4.0
$ cd libstdc++-v3
```

# STL组成

```mermaid
graph LR
A{STL} --> B("containers") 
	B--> B1("array")
	B--> B2("vector")
	B--> B3("list")
	B--> B4("deque")
	B--> B5("set/unordered_set/multiset/unordered_multiset")
	B--> B6("map/unordered_map/multimap/unordered_multimap")
A --> C("algorithms")
	C--> C1("sort")
	C--> C2("search")
	C--> C3("erase")
	C--> C4(...)
A --> D("iterators")
	D--> D1("todo")
A --> E("functors")
A --> F("adapters")
A --> G("alloocator")

```

## 容器

### vector

vector(动态数组)





