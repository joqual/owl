# 🦉 owl

### A lightweight, header-only C++ logging library

### Usage
Just include `owl.hpp` in your projects and start logging!

```cpp
#include "owl.hpp"

int main() {
    // Set the minimum level you want to log
    owl::Logger::get().set_min_level(owl::Level::INFO);

    // Start logging
    OWL_INFO("This is just info");
    OWL_WARN("This is a warning ...");
    OWL_CRITICAL("THIS IS A CRITICAL MESSAGE !!!");

    // Silence all logs
    owl::Logger::get().set_enabled(false);
    OWL_ERROR("This won't be logged.");

    return 0;
}
```

*"A wise old owl lived in an oak;<br>
The more he saw, the less he spoke;<br>
The less he spoke, the more he heard;<br>
Why can't we all be like that wise old bird?"*
