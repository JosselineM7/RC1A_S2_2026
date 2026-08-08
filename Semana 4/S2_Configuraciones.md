# Semana 2 - ejemplo Práctico

## Introducción a la CLI en Cisco Packet Tracer

### Objetivo

Familiarizar al estudiante con el uso básico de la interfaz de línea de comandos (CLI) en un dispositivo Cisco, comprendiendo los distintos modos de operación y ejecutando comandos administrativos esenciales.

---

## Modos de operación

1. Accede al modo usuario privilegiado:

```
enable
```

2. Observa el cambio del prompt:

* `>` modo usuario
* `#` modo privilegiado

---

## Configuración básica

1. Ingresa al modo de configuración global:

```
configure terminal
```

2. Asigna un nombre al dispositivo:

```
hostname SW1
```

3. Desactiva la búsqueda de dominios Desactiva la resolución de nombres DNS en la consola, evitando retrasos cuando se escriben comandos incorrectos.:

```
no ip domain-lookup
```

4. Configura una contraseña cifrada:

```
enable secret Redes1
```

---

## Mensaje de advertencia

1. Configura el mensaje MOTD:

```
banner motd #Acceso solo para personal autorizado#
```

2. Sal del modo configuración:

```
exit
```

---

## Verificación de la configuración

1. Muestra la configuración actual:

```
show running-config
```

2. Entra nuevamente a configuración:

```
configure terminal
```

3. Ejecuta el comando `show` sin salir:

```
do show running-config
```

4. Sal al modo privilegiado:

```
exit
```

---

## Fecha y hora del dispositivo

**Este comando se ejecuta en modo privilegiado (`#`)**

1. Verifica la hora actual:

```
show clock
```

2. Configura la fecha y hora:

```
clock set 14:42:00 08 Aug 2026 
```

3. Verifica nuevamente:

```
show clock 15:30:00 07 Feb 2026
```

---

## Guardar configuración

1. Guarda los cambios realizados:

```
write memory
```
