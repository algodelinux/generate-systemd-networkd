# generate-systemd-networkd

Función
-----------

Script para generar el fichero /etc/netplan/01-systemd-networkd.yaml. Este script detecta las interfaces de red levantadas y las configura mediante el renderer networkd para obtener una dirección IP vía DHCP, habilitando WOL para permitir que los equipos se enciendan por red y aplicando la configuración una vez generado el fichero.

Recomiendo revisar el fichero /etc/netplan/01-systemd-networkd.yaml y el directorio /etc/netplan, por si tuviérais algún otro fichero de configuración.

Instalación
-----------

La forma más sencilla de instalarlo es ejecutar estos comandos en la máquina donde queramos disponer del script:  

   wget --no-check-certificate -O /usr/local/sbin/generate-systemd-networkd https://raw.githubusercontent.com/algodelinux/generate-systemd-networkd/master/generate-systemd-networkd  
   chmod 755 /usr/local/sbin/generate-systemd-networkd
  

Uso                   
---

   generate-systemd-networkd
