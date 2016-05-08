###Ejemplos de Python Y entornos Virtuales
=====================================

+ Instalar Python 2.7
+ Instalar Python 3.5.1 


###Comando py en Windows

Antes teniamos que hacer algo como esto 

```
C:\Python2.7\lib\python.exe --version
Python 2.7.11
C:\Python3.4\lib\python.exe --version
Python3.4
```

Ahora hacemos esto con Py Launcher en Windows 7/8/8.1/10

```
py -2   -m pip install SomePackage  # default Python 2
py -2.7 -m pip install SomePackage  # specifically Python 2.7
py -3   -m pip install SomePackage  # default Python 3
py -3.4 -m pip install SomePackage  # specifically Python 3.4
```
###Comando virtualenv

```
py -2   -m pip install virtualenv  # default Python 2
py -2.7 -m pip install virtualenv  # specifically Python 2.7
py -3   -m pip install virtualenv  # default Python 3
py -3.4 -m pip install virtualenv  # specifically Python 3.4
```

###Creando Entornos virtuales
```
py -2   -m virtualenv entornoNombre  # default Python 2
py -2.7 -m virtualenv entornoNombre2.7  # specifically Python 2.7
py -3   -m virtualenv entornoNombre3  # default Python 3
py -3.4 -m virtualenv entornoNombre3.4  # specifically Python 3.4
```


###Activando Entornos
```
c:\env\entorno2.7\Scripts\activate
o
c:\env\entorno3.5\Scripts\activate

```

###Desactivandolos

Se escribe "deactivate" en cualquier parte que estemos si esta habiliado un entorno lo cerrara

```
deactivate

```

###Comprobando Versiones

La ventaja es que ya no necesitamos sobreponer python -m, ya que esta implicito que es la de la version del python que pusismos pero supongamos es una maquina y nos dicen instala los paquetes en la maquina virtual, y queremos saber que version de python y de pip hacemos lo siguiente:

```
python --version
Python 2.7.11
python -m pip --version
pip 8.1.1 from C:\env\entorno2.7\lib\site-packages (python 2.7)
```
### Verificando Paquetes instalados

```
python -m pip list
	Django (1.9.2)
	pip (8.1.1)
	setuptools (21.0.0)
	wheel (0.29.0)
```


###Instalando Paquetes

```
python -m pip install django==1.9.2  #Instala la version 1.9.2
o  
python -m pip install django  		#instala la ultima version de django

```