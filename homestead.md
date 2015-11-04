# HOMESTEAD

#### INSTALACIÓN
1) Instalar virtualbox
https://www.virtualbox.org/

2) Instalar vagrant
https://www.vagrantup.com/

3) Instalar Homestead
```bash 
$vagrant box add laravel/homestead
```

4) Crear archivo .homestead y carpeta homestead
```bash 
$composer global require "laravel/homestead=~2.0"
```

5) Configuración (Correr comando dentro de la carpeta homestead)
```bash 
$ cd ~/.composer/vendor/laravel/homestead/ 
$ bash init.sh
```


####CREAR MAQUINA VIRTUAL
1) Crear host en tu pc (192.168.10.10 es la ip que usa generalmente vagrant y virtualbox)
```bash 
$vim /etc/hosts
```
Crear el host
192.168.10.10   demo.app
(demo.app es el -map del archivo homestead.yamel donde configuramos el site en el siguiente paso)

2) $homestead edit (abre el archivo homestead.yml para configurar las maquinas virtuales)
Ejemplo:
```bash 
folders:
    - map: ~/Projects (carpeta local dentro de tu usuario)
      to: /home/vagrant/Projects (carpeta dentro de la maquina virtual) 
sites:
    - map: demo.app (host)
      to: /home/vagrant/Projects/Demo (carpeta dentro de la maquina virtual) 
```

3)Crea la maquina virtual tomando los cambios en el archivo homestead.yaml en virtual box
```bash 
$homestead provision
```
