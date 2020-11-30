# ouster_os1
## ouster os1 라이다 센서 사용방법
### Use environment
  - ubnutu 16.04
  - ros kinetic 
### Setting the ouster os1 lidar sensor
#### 1. connect with pc pc와 연결
#### 2. network setting  네트워크 설정
#### 3. create workspace
 - http://wiki.ros.org/ko/catkin/Tutorials/create_a_workspace
#### 4. terminal 터미널
cd workspace/src
git clone https://github.com/ouster-lidar/ouster_example.git
cd ..
catkin_make
#### 5. Network dependent change
