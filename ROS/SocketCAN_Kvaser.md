# 1. Install tools
```shell
sudo apt-get install can-utils
sudo apt-get install net-tools
sudo apt-get install libmuparser-dev
```

# 2. Download ros_canopen package
```shell
git clone https://github.com/ros-industrial/ros_canopen.git
```

# 3. Connect Kvaser to PC
**After connect Kvaser to PC**
```shell
sudo modprobe can    
sudo modprobe kvaser_usb    
sudo ip link set can0 type can bitrate 500000    
sudo ifconfig can0 up
```

## 3. 1. Logically disconnect Kvaser device
```shell
sudo ifconfig can0 down
```

## 3. 2. Logically reconnect Kvaser device
```shell
sudo ifconfig can0 up
```

## 3. 3. Check can data
```shell
candump can0
```

# 4. Publish CAN raw data to ROS
```shell
rosrun socketcan_bridge socketcan_bridge_node
```
> Does canopen package need to be built?
