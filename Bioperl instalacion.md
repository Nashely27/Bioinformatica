
# Instalación de BioPerl en Ubuntu 18.04.2 LTS 64 Bits

Para comenzar la instalación de BioPerl en nuestro computador con Ubuntu seguimos lo siguientes comandos en la terminal:

    sudo apt-get update
    sudo apt-get install bioperl
  
  Después de la instalación de la paqueteria se requerirá configurara, para eso ejecutamos el siguiente comando:
  

    cpan BIo::Seq
   Nos apareceran algunas lineas en la terminal el final que diran algo como lo siguiente:
   

> What approach do you want?  (Choose 'local::lib', 'sudo' or 'manual')
 [local::lib]


A lo que nosotros respondemos con 

    sudo
Esperamos hasta que termine el proceso y ya tendremos instalado Bioperl en nuestra PC.

