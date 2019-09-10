# Instalación de FastQC-CUTADPT-TrimGalore-SPAdes-Velvet-CShell-MUMmer en Ubuntu 18.04.2 LTS
**Instalacion de FastQC**

Simplemente ejecutamos el siguiente comando

	sudo apt-get install fastqc


**Instalación de CUTADPT**
Antes de instalar este paquete es necesario contar en la el módulo *pip3* de Python 3 que se instala con el siguiente comando:

    sudo apt install python3-pip
Para instalar CUTADPT ingresamos el siguiente comando:

    pip3 install --user --upgrade cutadapt
  Revisamos que se instaló correctamente ejecutando el siguiente comando:
  

      ~/.local/bin/cutadapt --help
**Instalación de Trim Galore**
Vamos a instalar este paquete por medio de Python Anaconda, pero usaremos una versión mas ligera llamada Miniconda y se instalará como sigue:

Una vez descargado el instalado desde el siguiente [enlace](https://docs.conda.io/en/latest/miniconda.html) nos vamos a la carpeta donde se descargó y ejecutaremos el siguiente comando:

    bash Miniconda3-latest-Linux-x86_64.sh
  Nos aparecerá un asistente de instalación, terminamos y luego vamos a la siguiente ruta en la terminal:
  

    ~/miniconda3/compiler_compat
  
   Para verificar la instalación de Miniconda, en esa ruta ejecutamos el siguiente comando`
   

    conda list


Ahora ejecutamos el siguiente comando para instalar Trim Galore:

    conda install -c bioconda trim-galore


**Instalación de SPAdes**
Simplemente ingresamos el siguiente comando a la terminal:

    sudo pat-get install spades
  Y verificamos la instalación con la siguiente línea:
  

    spades.py --test
**Instalación de Velvet**
Ingresamos la siguiente línea a la terminal

    sudo apt-get install velvet
  **Instalación de C-Shell**
  Podemos instalar cualquiera de la dos versiones con las siguientes líneas:
  

    sudo apt-get install csh
o

    sudo apt-get install tsch
  y testeamos escribiendo en la terminal: `csh`o `tsch`dependiendo de cual hallamos instalado.
  **Instalación de MUMmer**
  Descargamos el archivo *.tar.gz* desde el siguiente enlace:
  [Descarga MUMmer](https://sourceforge.net/projects/mummer/files/)
 y extraemos los archivos con el comando:
 

    tar -xvzf MUMmer3.0.tar.gz
Después de la extracción ejecutamos la siguiente línea:

    make check
finalmente:

    make install
y así ya tendremos instalado nuestro paquete.
