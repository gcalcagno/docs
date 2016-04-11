#HOMESTEAD

##INSTALACIÓN

1) Instalar virtualbox https://www.virtualbox.org/
#
2) Instalar vagrant https://www.vagrantup.com/
#
3) Instalar Homestead
$vagrant box add laravel/homestead
#
4) Crear archivo .homestead y carpeta homestead
$composer global require "laravel/homestead=~2.0"
#
5) Configuración (Correr comando dentro de la carpeta homestead)
$ cd ~/.composer/vendor/laravel/homestead/
$ bash init.sh
#

##NUEVO PROYECTO
1) $vim /etc/hosts
#
Crear host  (192.168.10.10 es la ip que usa generalmente vagrant y virtualbox)
#
2) $homestead edit 
#
(abre el archivo homestead.yml para configurar las maquinas virtuales) Ejemplo:
#
folders:
#
­map: ~/Projects (carpeta local dentro de tu usuario)
#
to: /home/vagrant/Projects (carpeta dentro de la maquina virtual)
#
sites:
#
­map: demo.app (host)
#
to: /home/vagrant/Projects/Demo (carpeta dentro de la maquina virtual)
#
3) $vagrant provision
#
Actualiza los cambios en el archivo homestead.yaml en virtual box
#


##ENCENDER MAQUINA VIRTUAL
vagrant up
