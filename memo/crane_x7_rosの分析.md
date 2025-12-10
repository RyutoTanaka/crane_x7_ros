# crane_x7_rosを読み解こう

ROS2の勉強はTF2まで終わった状態でCRANE-X7を動かしたけど、何もわからない〜
どこがわからないのか分析するために、crane_x7_rosの構造とか依存関係とかを読み解こう！

## crane_x7_rosのパッケージ

craneのプログラムを理解するためには、以下の要素について理解する必要がありそう

#### 内部パッケージ
- crane_x7_control
- crane_x7_examples
- crane_x7_gazebo
- crame_x7_moveit_config
- crane_x7_description（外部）

#### 依存関係
- rt_manipulators_cpp
- ros2_control
- Moveit 2

## 構造
1. examples
2. Moveit 2
3. ros2_control
4. x7_control

Moveitはロボットの軌道生成に関するフレームワーク、軌道・速度を生成する
ROS2_controlはロボットの制御を行うフレームワーク、軌道司令にロボットを追従させる
x7_controlはハードウェアを抽象化するプログラム、ROS2_controlの先っぽ










