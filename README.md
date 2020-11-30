# ouster_os1
## ouster os1 라이다 센서 사용방법
### Use environment
  - ubnutu 16.04
  - ros kinetic 
### Setting the ouster os1 lidar sensor
#### 1. connect with pc  pc와 연결
#### 2. network setting   네트워크 설정
#### 3. create workspace
 - http://wiki.ros.org/ko/catkin/Tutorials/create_a_workspace
#### 4. terminal 터미널
  ```
  $cd workspace/src
  $git clone https://github.com/ouster-lidar/ouster_example.git
  $cd ..
  $catkin_make
  ```

#### 5. Change the launch file for the network
- workspace/src/ouster_example/ouster_ros/os1.launch open
- Change default value  default 값 변경
  - os1_hostname is the ouster address  os1_hostname은 ouster 주소(192.168.1.201)
  - os1_udp_dest is the ethernet address(You can use the address you set when setting up the network.)  
    os1_udp_dest는 이더넷 주소(네트워크 설정할 때 설정한 주소로 하면된다.)

### Running the ouster os1 lidar sensor
  - terminal
  ```
  $cd workspace
  $source devel/setup.bash
  $cd src/ouster_example/ouster_ros
  $roslaunch os1.launch
  ```
  
  - View as visualization
  
  ```
  $rviz -d viz.rviz
  ```
  - Setting rviz
   ```
   add
   By topic
   PointCloud2
   ```
  
