# C++Server
# C++基础
[C++运行的原理]()
🎉🎉🎉
[C++的构造函数和析构函数]()
🎉🎉🎉
[指针和引用]()
🎉🎉🎉
[类型转换]()
🎉🎉🎉
[手动申请内存]()
🎉🎉🎉
[STL]()
🎉🎉🎉
[多线程]()
🎉🎉🎉
[数据结构]()
🎉🎉🎉
[网络编程]()
🎉🎉🎉
[linux命令]()
🎉🎉🎉
[gdb调试]()
🎉🎉🎉

这是一份非常全面、结构化、且面向职业发展的 **C++ & Linux 后端开发全栈知识图谱**。我将其整理为 Markdown 格式，方便你复制保存或导入笔记软件（如 Notion、Obsidian）。

---

# 🚀 C++ 全栈开发路线图：从入门到架构师

这份路线图涵盖了从 C++ 语言基础、现代 C++ 特性、标准库、底层原理，到 Linux 系统编程、网络编程以及最终的项目实战。

---

## 📅 第一阶段：语言基础 (Foundation)
> **目标**：建立正确的 C++ 编程思维，区分 C 与 C++，掌握内存模型。

### 1.1 C++ 基础语法
- [ ] **数据类型与变量**：整型、浮点型、字符型、布尔型、作用域。
- [ ] **流程控制**：if/else, switch, for/while, break/continue。
- [ ] **函数**：函数声明与定义、参数传递（值传递 vs 引用传递）、默认参数、函数重载。
- [ ] **指针与引用 (核心)**：
    - 指针的本质（内存地址）。
    - 引用（别名）与指针的区别。
    - `const` 指针 vs 指向 `const` 的指针。
    - 二级指针与数组指针。

### 1.2 内存管理初步
- [ ] **内存分区**：栈 (Stack)、堆 (Heap)、全局/静态区、常量区、代码区。
- [ ] **动态内存分配**：
    - `new` / `delete` vs `malloc` / `free`。
    - 内存泄漏 (Memory Leak) 的概念。
    - 深拷贝与浅拷贝（Deep Copy vs Shallow Copy）。

### 1.3 面向对象编程 (OOP)
- [ ] **类与对象**：`class` vs `struct`，`this` 指针。
- [ ] **封装**：`public` / `private` / `protected`。
- [ ] **特殊成员函数**：构造函数、析构函数、拷贝构造函数、赋值运算符重载。
- [ ] **继承**：基类与派生类、继承方式、多重继承（菱形继承问题）。
- [ ] **多态 (Polymorphism)**：
    - 虚函数 (`virtual`)。
    - **底层原理**：虚函数表 (vtable) 与 虚指针 (vptr)。
    - 纯虚函数与抽象类 (Interface)。

> 🔗 **参考资源**：
> *   [C++ 官方参考文档 (CppReference)](https://zh.cppreference.com/) - 必收录
> *   [LearnCpp (英文优质教程)](https://www.learncpp.com/)

---

## 🛠️ 第二阶段：标准库与泛型编程 (STL)
> **目标**：不造轮子，熟练使用标准组件，理解数据结构。

### 2.1 泛型编程 (Templates)
- [ ] **函数模板**：参数推导。
- [ ] **类模板**：实现泛型容器。
- [ ] **模板特化**：全特化与偏特化。

### 2.2 STL 六大组件
- [ ] **容器 (Containers)**：
    - **序列式**：`std::vector` (动态数组扩容机制), `std::list` (双向链表), `std::deque`。
    - **关联式**：`std::map` / `std::set` (底层红黑树), `std::multimap`。
    - **无序式**：`std::unordered_map` / `std::unordered_set` (底层哈希表)。
- [ ] **迭代器 (Iterators)**：迭代器失效场景，`begin()`, `end()`。
- [ ] **算法 (Algorithms)**：`std::sort`, `std::find`, `std::transform`, `std::for_each`。
- [ ] **适配器**：`std::stack`, `std::queue`, `std::priority_queue` (堆)。

---

## ⚡ 第三阶段：现代 C++ (Modern C++ 11/14/17/20)
> **目标**：掌握现代 C++ 能够极大提高开发效率和安全性，是**面试重灾区**。

### 3.1 资源管理 (RAII)
- [ ] **智能指针** (彻底抛弃裸指针)：
    - `std::unique_ptr`：独占所有权。
    - `std::shared_ptr`：引用计数原理，`make_shared`。
    - `std::weak_ptr`：解决 `shared_ptr` 循环引用问题。

### 3.2 性能优化特性
- [ ] **移动语义 (Move Semantics)**：
    - 左值 (L-value) vs 右值 (R-value)。
    - 右值引用 `&&`。
    - `std::move` 与 移动构造函数。
    - **完美转发**：`std::forward`。

### 3.3 易用性特性
- [ ] `auto` 类型推导 与 `decltype`。
- [ ] Lambda 表达式 (匿名函数与闭包)。
- [ ] `nullptr` 替代 `NULL`。
- [ ] 范围 `for` 循环 (`for (auto& x : container)`).
- [ ] `std::function` 与 `std::bind`。

### 3.4 并发编程 (C++11 Concurrency)
- [ ] `std::thread` 管理线程。
- [ ] `std::mutex`, `std::unique_lock`, `std::lock_guard`。
- [ ] `std::atomic` 原子操作。
- [ ] `std::condition_variable` 条件变量。
- [ ] `std::future` 与 `std::async`。

---

## 🐧 第四阶段：Linux 系统编程 (System Programming)
> **目标**：理解代码如何在操作系统内核之上运行。

### 4.1 开发环境与工具链
- [ ] **编辑器**：Vim / VS Code (Remote-SSH)。
- [ ] **编译器**：GCC / G++ 编译流程 (预处理->编译->汇编->链接)。
- [ ] **调试器**：GDB (断点、单步、查看内存、调试 Core Dump)。
- [ ] **构建工具**：
    - **Makefile**：编写规则。
    - **CMake**：现代 C++ 项目标配 (`CMakeLists.txt`)。
- [ ] **版本控制**：Git。

### 4.2 进程与线程
- [ ] **进程管理**：`fork()`, `exec()`, `wait()`, `exit()`.
- [ ] **特殊进程**：孤儿进程、僵尸进程、守护进程。
- [ ] **进程间通信 (IPC)**：
    - 管道 (Pipe/FIFO)。
    - 共享内存 (Shared Memory) + 信号量 (Semaphore)。
    - 消息队列 (Message Queue)。
- [ ] **Linux 线程**：POSIX Threads (`pthread` 库) vs C++ `std::thread`。

### 4.3 文件与信号
- [ ] **文件 I/O**：文件描述符 (fd)，`open`, `read`, `write`, `lseek`, `fcntl`。
- [ ] **IO 重定向**：`dup`, `dup2`。
- [ ] **信号 (Signal)**：信号注册 `signal`/`sigaction`，常用信号 `SIGINT`, `SIGKILL`, `SIGTERM`。

---

## 🌐 第五阶段：Linux 高性能网络编程 (Network)
> **目标**：这是后端开发的**核心**，决定了你能不能写出高并发服务器。

### 5.1 网络基础
- [ ] **TCP/IP 协议栈**：IP, TCP, UDP。
- [ ] **TCP 状态机**：三次握手、四次挥手、TIME_WAIT 状态。
- [ ] **Socket 编程**：`socket`, `bind`, `listen`, `accept`, `connect`。
- [ ] **字节序**：大端序 (Big Endian) vs 小端序。

### 5.2 高并发 I/O 模型 (重点)
- [ ] **阻塞 I/O (Blocking)** vs **非阻塞 I/O (Non-Blocking)**。
- [ ] **I/O 多路复用 (IO Multiplexing)**：
    - `select` (缺点)。
    - `poll`。
    - **`epoll`** (Linux 核心神器)：ET (边缘触发) vs LT (水平触发) 模式。

### 5.3 高性能服务器模型
- [ ] **Reactor 模型**：事件循环 (Event Loop) + 非阻塞 IO + Epoll。
- [ ] **Proactor 模型**：异步 IO (AIO)。
- [ ] **线程池 (Thread Pool)**：避免频繁创建销毁线程。
- [ ] **常见网络库分析**：Muduo, Libevent, Boost.Asio。

> 🔗 **必读经典**：
> *   [Beej's Guide to Network Programming (网络编程入门神书)](https://beej.us/guide/bgnet/)

---

## 🏗️ 第六阶段：进阶话题与架构
- [ ] **设计模式**：单例 (Singleton, 线程安全版)、工厂 (Factory)、观察者 (Observer)。
- [ ] **内存池 (Memory Pool)**：减少 malloc 调用，防碎片。
- [ ] **RPC 原理**：Protocol Buffers (序列化), gRPC。
- [ ] **数据库接口**：MySQL Connector/C++, Redis (hiredis)。
- [ ] **C++20 新特性**：协程 (Coroutines), Modules, Concepts。

---

## 💻 第七阶段：项目实战 (Projects)
> **建议**：不仅要写，还要上传 GitHub，并写好 Readme。

### 7.1 入门级：手写 STL 容器
*   **描述**：自己实现一个 `MyVector` 或 `MyString`。
*   **涉及知识**：动态内存管理、模板、运算符重载、迭代器。

### 7.2 进阶级：HTTP Web 服务器 (Web Server)
*   **描述**：在 Linux 下实现一个高性能 Web 服务器，解析 HTTP 请求并响应。
*   **涉及知识**：
    *   Epoll 边缘触发 + 非阻塞 IO。
    *   线程池处理业务逻辑。
    *   状态机解析 HTTP 报文。
    *   定时器处理非活动连接。
*   **参考项目**：
    *   [TinyWebServer (GitHub 高星项目)](https://github.com/qinguoyi/TinyWebServer)

### 7.3 专家级：分布式 KV 存储 / RPC 框架
*   **描述**：实现一个简单的键值数据库或远程调用框架。
*   **涉及知识**：网络序列化 (Protobuf)、Raft 一致性算法、LSM-Tree 存储引擎、Zookeeper。
*   **参考项目**：
    *   [Muduo 网络库](https://github.com/chenshuo/muduo)
    *   [MIT 6.824 (分布式系统课程)](https://pdos.csail.mit.edu/6.824/)

---

## 📚 推荐书单 (Roadmap Books)

1.  **入门**：
    *   📖 《C++ Primer》 (第5版) —— *不要看 Primer Plus，直接看这本*。
2.  **进阶**：
    *   📖 《Effective C++》 —— *必读，教你避坑*。
    *   📖 《STL 源码剖析》（侯捷） —— *理解容器底层*。
3.  **Linux/网络**：
    *   📖 《Linux 高性能服务器编程》（游双） —— *最适合入门网络编程的书*。
    *   📖 《UNIX 环境高级编程 (APUE)》 —— *案头字典*。
4.  **底层**：
    *   📖 《深度探索 C++ 对象模型》 —— *面试高频*。

---

### 💡 学习建议
1.  **多调试**：不要光看书，多用 GDB 调试，查看内存和寄存器。
2.  **看源码**：阅读优秀的开源项目（如 Nginx, Redis, LevelDB）的 C/C++ 源码。
3.  **造轮子**：尝试复现标准库的功能，这是提升最快的方法。
