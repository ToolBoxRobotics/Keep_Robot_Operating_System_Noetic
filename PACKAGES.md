
## ROS Noetic Rosserial Arduino

#### Install packages
```terminal
sudo apt-get install ros-noetic-rosserial-arduino
rosdep install rosserial_arduino
rosdep update
```

#### Lancez le roscore
```terminal
roscore
```
#### Exécutez l'application client rosserial qui transfère vos messages Arduino au reste de ROS. Assurez-vous d'utiliser le bon port série. 
```terminal
rosrun rosserial_python serial_node.py
```

#### Alternativement, si vous voulez pouvoir réinitialiser votre Arduino par programmation, exécutez en utilisant
```terminal
rosrun rosserial_arduino serial_node.py _port:=/dev/ttyACM0
```


