# ALGUNOS COMANDOS EN CMD

```shell
# PROBLEMA A LA HORA DE ACCEDER A LOCALHOST
# DAR PRIVILEGIOS A USUARIOS SOBRE LA CARPETA apache-tomcat-9.0.53
```

```shell
# dir = listar
# type = leer
```

```shell
C:\Program Files\Apache Software Foundation\apache-tomcat-9.0.53\bin>catalina start
# Arranca el servidor
C:\Program Files\Apache Software Foundation\apache-tomcat-9.0.53\bin>catalina stop
# Para el servidor
```

## TomCat

### 1. TomCat versiones necesarias

- Debemos tener dos programas TomCat, uno para NetBeans y otro para Manager-Aplication.
- Para Netbeans tengo la versión: 9.0.14
- Para App tengo la versión: 9.0.53

### 2. Configuración de TomCat para Manager App

```shell
# CREAR USUARIO ADMINISTRADOR
# apache-tomcat-versionX/conf/tomcat-users.xml
# USERNAME + PASSWORD + ROL 
<role rolename="manager-gui"/>
<role rolename="manager-script"/>
<role rolename="admin"/>
<user password="secreto" roles="manager-gui, manager-script" username="admin"/>
```

### 3. Configuración en NetBeans

#### CONFIGURACIÓN SERVIDOR

- Abrir NetBeans y seleccionar del menú de navegación superior ``windows / services ``. Se abrirá una ventana a la izquierda (junto a Projects y Files). Seleccionar con clic derecho ``servers``:

![image](https://user-images.githubusercontent.com/82242888/134365342-1969c848-310f-437d-a1ea-2c90ecd790e7.png)

![image](https://user-images.githubusercontent.com/82242888/134365589-572e817a-2b5b-4fde-bada-d74aee9e6390.png)


- Seleccionamos la carpeta (nosotros no instalamos TomCat en el terminal, pero si lo hiciésemos, por defecto crea una carpeta ``Apache Software Fundation`` en Archivos de Programa, yo la he creado manualmente y he colocado ahí las distintas versiones de TomCat que tengo para trabajar):
![image](https://user-images.githubusercontent.com/82242888/134365932-86ac2337-d177-4a33-bf72-ea7e433c00cf.png)



- Introducimos USERNAME y PASSWORD (estos serán los requeridos al iniciar el servidor en NetBeans, no confundir con la contraseña y nombre dados para el TomCat de Manager):

 ![image](https://user-images.githubusercontent.com/82242888/134366005-67d2987c-4fe1-4bc7-8936-5058b94aad1c.png)
 ![image](https://user-images.githubusercontent.com/82242888/134366090-5b4dcf3c-cd89-4213-9224-34d48d37d3a3.png)


#### NUEVO PROYECTO

![image](https://user-images.githubusercontent.com/82242888/134366168-1b997deb-a8c1-416f-a3ab-21833bc90a3c.png)

![image](https://user-images.githubusercontent.com/82242888/134366240-09779ac4-c43b-45e8-9857-28d0671facf1.png)

![image](https://user-images.githubusercontent.com/82242888/134366288-c1858ba4-6100-45f7-a122-c003f6f8890c.png)
