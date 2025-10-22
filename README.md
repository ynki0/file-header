# file-header
Convert any binary to a C-style array (generating an header file)

# Usage
```
$ file2header <input_binary.exe> <output_header.h> <bytes_per_line>
```
```
<input_binary.exe>    Path to any binary file
<output_header.h>     Path to output file
<bytes_per_line>      Optionnal: Number of bytes for each line (default: 25)
Example: file header image.exe image.h 30
```
# Output example
```c++
#pragma once
#include <cstdint>

const uint8_t image[] = 
{
    0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00 //...
};
```
