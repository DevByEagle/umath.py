# Xalloc - A High-Performance Memory Allocator

`xalloc` is a custom memory allocator designed for high performance, low overhead, and flexibility in memory management for C and C++ projects. This allocator is optimized to handle allocation and deallocation of memory efficiently, minimizing fragmentation and improving runtime performance.

## Features

- **Customizable:** Easily configurable to suit different use cases and system requirements.
- **Cross-Platform:** Works on any platform with a C compiler, allowing seamless integration into projects across various operating systems.

## Usage

```c
#define MEMORY_SIZE 1024 * 1024
#include "xalloc.h"

int main() {
    int* arr = (int*)xalloc(10 * sizeof(int));

    // Use the memory...
    
    xfree(arr);

    return 0;
}
```
