
# sistema-OSI-Resolucion
Cómo resolver y documentar el sistema OSI

![GitHub Stats](V1.jpg)

📌 Cómo resolver y documentar el sistema OSI
La idea es que cada capa tenga:

Definición breve (qué hace).

Ejemplo práctico (comando o herramienta que la valida).

Captura (salida real de tu laboratorio).

Observación (qué significa el resultado).

📊 Ejemplo de documentación por capas
Capa Física

Definición: cables, señal, hardware.

Ejemplo: revisar conexión en VirtualBox (adaptador habilitado).

Observación: si el cable virtual no está conectado, no hay tráfico.

Capa Enlace de Datos

Definición: direcciones MAC, switches.

Ejemplo: ip link show en Linux.

Observación: interfaz activa con MAC válida.

Capa Red

Definición: direccionamiento IP, rutas.

Ejemplo:  ip route show, ping 8.8.8.8.

Observación: si falla, revisar gateway o adaptador.

Capa Transporte

Definición: TCP/UDP, puertos.

Ejemplo: netstat -tulnp o ss -tulnp.

Observación: servicio escuchando en puerto correcto.

Capa Sesión

Definición: control de sesiones entre aplicaciones.

Ejemplo: conexión SSH (ssh usuario@host).

Observación: sesión establecida correctamente.

Capa Presentación

Definición: formato de datos, cifrado.

Ejemplo: HTTPS (certificados válidos).

Observación: datos interpretados correctamente.

Capa Aplicación

Definición: servicios visibles al usuario.

Ejemplo: curl google.com.

Observación: respuesta HTTP válida.

### 📚 Sistema OSI – Documentación práctica

Cada capa se valida con comandos y capturas:

- Física → VirtualBox adaptador habilitado.  
- Enlace → `ip link show`.  
- Red → `ping 8.8.8.8`.  
- Transporte → `netstat -tulnp`.  
- Sesión → conexión SSH.  
- Presentación → HTTPS válido.  
- Aplicación → `curl google.com`.

📌 Observación: Documentar cada capa permite ubicar el fallo en el nivel correcto y aplicar la reparación adecuada.


