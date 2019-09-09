# Instalación de CPP, Quast y SAMtools en Ubuntu 18.04.2 LTS
**Instalacion de CPP**
Solo basta con ejecutar el siguiente comando en la terminal

    sudo apt-get install gcc
Para saber que ya está instalado ingresamos el siguiente comando en la terminal:

    gcc --version
**Instalación de Quast**
Antes de comenzar la instalación asegúrese de tener los siguientes paquetes instalados en su ordenador:

Python2 (2.5 or higher) or Python3 (3.3 or higher)
-   GCC 4.7 or higher
-   Perl 5.6.0 or higher
-   GNU make and ar
-   zlib development files

Para instalar la libreria *zliblg* ingresamos el siguiente comando:

    sudo apt-get install zlib1g-dev
También se necesita una librería de Python llamada *matplotlib* y para instalarla ingresamos el siguiente comando:

    sudo apt-get install -y pkg-config libfreetype6-dev libpng-dev python-matplotlib
    
 
Ahora descargamos y descomprimimos Quast con el siguiente comando:

    wget https://downloads.sourceforge.net/project/quast/quast-5.0.2.tar.gz
    tar -xzf quast-5.0.2.tar.gz
    cd quast-5.0.2
Para instalarlo ejecutamos el siguiente comando:

    ./setup.py install
Podemos verificar si se instaló correctamente ejecutando el siguiente comando:

    ./quast.py test_data/contigs_1.fasta \
               test_data/contigs_2.fasta \
               -r test_data/reference.fasta.gz \
               -g test_data/genes.gff
**Instalación de SAMtools**
Solo basta con ingresar el siguiente comando a la terminal:

   

    sudo apt-get install samtools

