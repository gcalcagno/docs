# HOMESTEAD

#### INSTALACIÓN
1) install virtualbox

2) install vagrant

3) $vagrant box add laravel/homestead

4) $composer global require "laravel/homestead=~2.0"
(crea .homestead y carpeta homestead)

5) 
```bash 
$ cd ~/.composer/vendor/laravel/homestead/ 
$ bash init.sh (correr este comando dentro de la carpeta homestead)
```

6)$homestead up
(crea la maquina virtual en virtual box)

CREAR MAQUINA VIRTUAL
1) Crear host
$vim /etc/hosts
Agregar la línea:
192.168.10.10   demo.app

7) $homestead edit (abre el archivo homestead.yml)
Ejemplo:
folders:
    - map: ~/Projects (carpeta local dentro de tu usuario)
      to: /home/vagrant/Projects (carpeta dentro de la maquina virtual) 
sites:
    - map: homestead.app (host)
      to: /home/vagrant/Projects (carpeta dentro de la maquina virtual) 
    - map: demo.app (host)
      to: /home/vagrant/Projects/Demo (carpeta dentro de la maquina virtual) 
