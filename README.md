# Praca inżynierska
#### Temat: Integracja bazy mobilnej z częścią manipulacyjną robota Velma na rzecz symulacji

### Środowisko symulacji
Symulator został przygotowany do pracy w następującym środowisku:
- System operacyjny Ubuntu 18
- dystrybucja ROS Melodic Morenia
- symulator Gazebo w wersji 9.4

### Przygotowanie środowiska 
W pierwszej kolejności należy w katalogu roboczym `~/catkin_ws/src` sklonować repozytorium za pomocą
polecenia `git clone https://github.com/RCPRG-ros-pkg/omnivelma.git`. Po sklonowaniu repozytorium należy przenieść
się do folderu głównego katalogu roboczego `cd ..` i zbudować symulator za pomocą polecenia `catkin_make`.
Po zbudowaniu, należy załadować środowisko symulatora za pomocą polecenia `source devel/setup.bash`.

### Uruchomienie symulatora bazy mobilnej
Aby uruchomić symulator bazy mobilnej należy przejść do katalogu `~/catkin_ws/src/omnivelma` i wykonać polecenie
`./launches/gazebo`. Spowoduje to uruchomienie się symulatora Gazebo wraz z załadowanym światem symulacji i bazą 
mobilną a takze uruchomienie się programu `lalkarz`, dzięki któremu w prosty sposób można sterować pojazdem 
za pomocą klawiatury numerycznej.
