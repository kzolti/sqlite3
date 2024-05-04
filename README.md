### SQLite3 Compiler

This repository provides a convenient way to compile specific versions of SQLite3 from its source code using CMake.

#### Usage:

For example, to compile SQLite3 version 3.8.10, use the following command:

1. Clone the repository:

   ```bash
   git clone https://github.com/kzolti/sqlite3.git && \
   cd sqlite3
    ```
2. Check build_options.txt to see the available options for SQLite3 version. For detailed information on available options, refer to [SQLite3 Compile-time Options](https://www.sqlite.org/compile.html). 


3. Create a build directory and run CMake:
```bash
mkdir build && cd build && \
cmake -DSQLITE_VERSION=3.8.10 .. && cmake --build .
```
#### Attention:
Include and target files are copied to CMAKE_CURRENT_SOURCE_DIR/include and CMAKE_CURRENT_SOURCE_DIR/target.    
#### Note:
This repository provides a convenient way to compile specific versions of SQLite3 from its source code using CMake.