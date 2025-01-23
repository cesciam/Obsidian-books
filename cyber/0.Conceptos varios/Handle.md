Handle del proceso: El handle es un identificador de acceso que se utiliza para interactuar con objetos del sistema. Ejemplo, puedo tener un HANDLE para interactuar con un file, un window, un proceso,etc. 
https://learn.microsoft.com/en-us/windows/win32/sysinfo/about-handles-and-objects

Cada objeto tiene su propio ACL, y cada vez que el sistema crea un handle, se verifica primero el acl de ese objeto. 