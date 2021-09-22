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

![image-20210916194807985](C:\Users\manue\AppData\Roaming\Typora\typora-user-images\image-20210916194807985.png)



### 3. Configuración en NetBeans

#### CONFIGURACIÓN SERVIDOR

- Abrir NetBeans y seleccionar del menú de navegación superior ``windows / services ``. Se abrirá una ventana a la izquierda (junto a Projects y Files). Seleccionar con clic derecho ``servers``:

![image-20210922161839374](C:\Users\manue\AppData\Roaming\Typora\typora-user-images\image-20210922161839374.png)



![image-20210922161500040](C:\Users\manue\AppData\Roaming\Typora\typora-user-images\image-20210922161500040.png)

- Seleccionamos la carpeta:

![image-20210922161615841](C:\Users\manue\AppData\Roaming\Typora\typora-user-images\image-20210922161615841.png)

- Introducimos USERNAME y PASSWORD (estos serán los requeridos al iniciar el servidor en NetBeans, no confundir con la contraseña y nombre dados para el TomCat de Manager):

  ![image-20210922161713701](C:\Users\manue\AppData\Roaming\Typora\typora-user-images\image-20210922161713701.png)

#### NUEVO PROYECTO

![image-20210922161003502](C:\Users\manue\AppData\Roaming\Typora\typora-user-images\image-20210922161003502.png)

![image-20210922161022484](C:\Users\manue\AppData\Roaming\Typora\typora-user-images\image-20210922161022484.png)

![image-20210922161057284](C:\Users\manue\AppData\Roaming\Typora\typora-user-images\image-20210922161057284.png)
