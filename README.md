# Estudando_ROS2
## Processo de instalação do ROS 2 jazzy para Ubundu 24.04 noble.

Siga os comandos abaixo para instalar o ROS2 Jazzy no Ubuntu 24.04:

````
locale
````
````
sudo apt update && sudo apt install locales
````
````
sudo locale-gen en_US en_US.UTF-8
````
````
sudo update-locale LC_ALL=en_US.UTF-8 LANG=en_US.UTF-8
````
````
export LANG=en_US.UTF-8
````
````
locale
````
Agora, em outro terminal:
````
sudo apt install software-properties-common
````
````
sudo add-apt-repository universe
````
````
sudo apt update && sudo apt install curl -y
````
````
sudo curl -sSL http://raw.githubusercontent.com/ros/rosdistro/master/ros.key -o /usr/share/keyrings/ros-archive-keyring.gpg
````
````
echo "deb [arch=$(dpkg --print-architecture)
signed-by=/usr/share/keyrings/ros-archive-keyring.gpg] http://packages.ros.org/ros2/ubuntu $(. /etc/os-release && echo $UBUNTU_CODENAME) main" | sudo tee /etc/apt/sources.list.d/ros2.list > /dev/null
````
````
sudo apt update && sudo apt install ros-dev-tools
````
Agora, em outro terminal:
````
sudo apt install ros-jazzy-desktop
````
````
echo "source /opt/ros/jazzy/setup.bash" >> ~/.bashrc
````
````
source ~/.bashrc
````
````
sudo apt-get install gedit -y
````
````
gedit ~/.bashrc
````
Pode fechar a janela que foi aberta.

Você pode usar usar os três comandos abaixo para checar que a versão instalada do ROS é o Jazzy:
````
printenv ROS_DISTRO
````
````
env | grep ROS
````
````
echo $ROS_DISTRO
````
````
````
````
````
````
````
````
````
````
````
````
````
````
````
````














































