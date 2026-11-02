Nustro proyecto de Fundamentos de computacion 
Nuestro proyecto en Markdown 

# Fundamentos de Computación

**Equipo:** Isabella Medina Molina y Franklin Jiménez Narváez

---

## Problemática

Las colonias y fraccionamientos enfrentan un deterioro severo de la infraestructura pública: calles y aceras dañadas, postes de luz sin funcionar, cortes constantes de luz y falta de agua.

---

## Objetivo y propuesta de solución

Ayudar a reportar y hacer más visibles los problemas estructurales y/o de servicio en las comunidades mediante la creación de una aplicación que permita a los usuarios reportar problemas de infraestructura pública.

La aplicación contará con las siguientes funciones:

- Mostrar un mapa de la ciudad en el cual se pueda seleccionar la ubicación exacta de la falla.
- Tomar una foto del problema.
- Describir el problema.

Una vez identificado el problema, el reporte se envía a los canales oficiales correspondientes del gobierno para su atención y seguimiento.

---

## División del trabajo

| Área                  | Responsable |
|-----------------------|-------------|
| Frontend              | Isabella    |
| Backend               | Franklin    |
| Base de datos         | Isabella    |
| Encargado de servidores | Franklin  |git

---

## Alcance:

### Frontend:
- Se muestra un mapa interactivo para elegir la ubicación exacta (pin arrastrable) y botón “usar mi ubicación actual”. Tomar una foto con la cámara o seleccionar una de galería.
- Llenar el formulario: categoría (bache, alumbrado, falta de agua, corte de luz, etc.), descripción del problema y la ubicación.
- Sección "mis reportes" y login/registro.
- Botón "Enviar problemática”.
- Estatus del reporte.
- Lenguajes: HTML, CSS y JavaScript

### Backend:
- Recibir y validar los reportes (foto, texto, coordenadas).
- Guardar la foto y los datos.
- Listar los reportes para mostrarlos en el mapa.
- Decidir a qué dependencia de gobierno corresponde cada reporte según su categoría.
- Enviar la notificación (correo, y después WhatsApp).
- Autenticación de usuarios y control de estatus (enviado, en proceso, resuelto).
- Detección de duplicados para no enviar 20 correos por el mismo bache.

### Base de datos:
- Usuarios: quién creó cada reporte.
- Categorías: bache, alumbrado, fuga de agua, basura, etc.
- Dependencias: cada oficina de gobierno con su correo y/o número de WhatsApp. Ejemplo:” CFE, +52 55 4195 7878 "
- Categoria_dependencia: si dice que "no hay luz" o “problemas de luz” se envía a "CFE".
- Notificaciones: registro de cada correo enviado, para saber si llegó o falló.

### Encargado de servidores: 
- Hosting


