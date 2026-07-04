# cmd-comandos-consultas
cmd comandos que he buscado personalmente para poder no sólo consultar, o hacer conceptos a nivel empresa.. 

usar **Tiny10**, aprender **CMD** 


```cmd
systeminfo
hostname
whoami
ipconfig /all
tasklist
driverquery
netstat -ano
wmic cpu get name
wmic memorychip get capacity
dir /O:-D
tree
```

Con esos ya puedes inspeccionar un equipo bastante bien sin instalar nada.


Lo básico:

```cmd
C:
```

Cambiar a la unidad C.

```cmd
D:
```

Cambiar a la unidad D.

---

Ver archivos de una carpeta:

```cmd
dir
```

---

Ver el contenido de C:

```cmd
dir C:\
```

o estando en C:

```cmd
dir
```

---

Entrar a una carpeta:

```cmd
cd Carpeta
```

Ejemplo:

```cmd
cd Users
cd Oscar
cd Documents
```

Volver atrás:

```cmd
cd ..
```

Ir hasta la raíz:

```cmd
cd \
```

---

### Ver fechas y tamaños

```cmd
dir
```

Ya muestra algo como:

```
04/07/2026  11:20 AM    <DIR>    Program Files
03/07/2026  08:15 PM              archivo.txt
```

Ahí ves:

* Fecha
* Hora
* Tamaño
* Nombre

---

### Ordenar por fecha

Más reciente primero:

```cmd
dir /O:-D
```

Más antiguo primero:

```cmd
dir /O:D
```

---

### Solo carpetas

```cmd
dir /AD
```

Solo archivos

```cmd
dir /A-D
```

---

### Buscar un archivo

Por nombre:

```cmd
dir *.exe /S
```

Busca todos los `.exe`.

Por ejemplo:

```cmd
dir ventoy* /S
```

o

```cmd
dir *.iso /S
```

`/S` significa **buscar en todas las subcarpetas**.

---

### Mostrar todo (incluyendo ocultos)

```cmd
dir /A
```

---

### Ver únicamente nombres

```cmd
dir /B
```

Queda así:

```
archivo.txt
foto.jpg
Windows
Program Files
```

---

### Árbol de carpetas

```cmd
tree
```

o

```cmd
tree /F
```

`/F` también muestra los archivos.

---

### Información del disco

```cmd
vol
```

o

```cmd
wmic logicaldisk get caption,freespace,size
```

En equipos recientes también puedes usar PowerShell:

```powershell
Get-Volume
```

---

### Saber dónde estás

```cmd
cd
```

o

```cmd
echo %cd%
```

---

