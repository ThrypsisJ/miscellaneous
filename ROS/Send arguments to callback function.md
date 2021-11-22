# Send arguments to callback function

* include **bind** function of **boost** libarary
```c++
#include <boost/bind.hpp>
```

* Declare/defind subscriber
```c++
ros::NodeHandle n;
ros::Subscriber sub = n.subscribe<Message type>("Topic name", Queue_size, boost::bind(&callbackfunction, _1, &argument1, &argument2, ...));
```

* If compiler can't find **boost** library
in CMakeList.txt
```cmake
find_package(Boost REQUIRED COMPONENTS thread)
include_directories($(Boost_INCLUDE_DIRS))
```
