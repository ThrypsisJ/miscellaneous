# Create custom message
## Create message file
### at package folder
```bash
mkdir msg
vi <message_name>.msg
```
※ See http://wiki.ros.org/msg to check data types

## Modify CMakeList.txt
```cmake
find_package(catkin REQUIRED_COMPONENTS
  message_generation
)

add_message_file(
  FILES
  <message_name>.msg
)

generate_messages(
  DEPENDENCIES
)
```

## Modify package.xml
```xml
<build_export_depend>message_runtime</build_export_depend>
<build_depend>message_generation</build_depend>
<exec_depend>message_runtime</exec_depend>
```

## Include msg file in source code
```C++
#include "<project_name>/<message_name>.h"

// optional
using <project_name>::<message_name>;
```
