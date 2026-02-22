## # Turtlebot3 Burger 설정
- 아래 로보티즈사이트로 접속하여 필요한 내용을 따라 함
- [ROBOTIS e-Manual](https://emanual.robotis.com/docs/en/platform/turtlebot3/quick-start/)

### Turtlebot3 burger의 WIFI_SSID와 WIFI_PASSWORD 수정

```
sudo nano /etc/netplan/50-cloud-init.yaml
```

### ros-base에는 데모가 빠져 있을 수 있으므로, 필요한 것만 추가 설치

```
sudo apt update
sudo apt install -y ros-humble-demo-nodes-cpp ros-humble-demo-nodes-py
source /opt/ros/humble/setup.bash
ros2 run demo_nodes_cpp talker
```
