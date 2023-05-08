# Tutorial Basico Instalação Oppenni
![Badge em Desenvolvimento](http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge)

## Instalação dos pacotes dependentes:
```
$ sudo apt-get install libopenni0 libopenni-dev
```

## Instalação dos pacotes no Workspace :
```
$ cd ~/catkin_ws/src
$ git clone https://github.com/ros-drivers/openni_launch
$ git clone https://github.com/ros-drivers/openni_camera
$ git clone https://github.com/ros-drivers/rgbd_launch.git
```

Checar as dependências com rosdep:
```
$ rosdep update
$ rosdep check --from-paths . --ignore-src --rosdistro noetic
$ rosdep install --from-paths . --ignore-src --rosdistro noetic -y
```

Compilando a workspace:
```
$ cd ~/catkin_ws/
$ catkin_make
```

Source:
```
$ source devel/setup.bash
```

Testando o launch:

```
$ roslaunch openni_launch openni.launch

```

## Configuração do oppenin_tracker

## Instalação dos pacotes no Workspace :
```
$ cd ~/catkin_ws/src
$ git clone https://github.com/ros-drivers/openni_tracker
```
Checar as dependências com rosdep:
```
$ rosdep update
$ rosdep check --from-paths . --ignore-src --rosdistro noetic
$ rosdep install --from-paths . --ignore-src --rosdistro noetic -y
```

Compilando a workspace:
```
$ cd ~/catkin_ws/
$ catkin_make
```

Source:
```
$ source devel/setup.bash
```

Instalamos o NITE-Bin-Dev-Linux-v1.5.2.23 na workspace:

```
$ cd catkin_ws
$ git clone https://github.com/arnaud-ramey/NITE-Bin-Dev-Linux-v1.5.2.23.git
```

Instalamos através de:

```
$ cd ~/catkin_ws/src/NITE-Bin-Dev-Linux-v1.5.2.23
$ cd x86/x64 (dependendo da arquitetura)
$ sudo bash install.sh
```
