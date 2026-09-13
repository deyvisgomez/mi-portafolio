# Guia de Documentacion: Laboratorio 03 - Trabajo Colaborativo con Repositorios Remotos

Documentacion oficial sobre el flujo de trabajo colaborativo en GitHub utilizando Fork, Clone, Issues y Pull Requests.

## Descripcion del Proyecto

Este laboratorio permite poner en practica el flujo de contribucion a un repositorio remoto existente. Se abordan la deteccion de errores en el codigo fuente, el reporte formal mediante Issues, la correccion en ramas independientes y la propuesta de integracion a traves de Pull Requests.

### Requisitos Previos

- Tener instalada y configurada la herramienta Git.
- Disponer de un editor de codigo como Visual Studio Code.
- Contar con una cuenta activa en GitHub con sesion iniciada.

---

## Pasos de Instalacion y Uso

### Configuracion del Entorno Local

1. Realizar un Fork del repositorio remoto hacia tu cuenta personal de GitHub.
2. Clonar el repositorio a tu equipo local ejecutando `git clone https://github.com/TU-USUARIO/tienda-tecsup.git`.
3. Acceder al directorio del proyecto e inspeccionar los remotos con el comando `git remote -v`.

### Checklist de Estado del Desarrollo

- [x] Correccion del calculo en el total del carrito (`script.js`)
- [x] Vinculacion del archivo de hojas de estilo (`index.html`)
- [ ] Sincronizacion final tras la revision del repositorio upstream

---

## Comandos y Archivos del Proyecto

| Archivo / Comando | Tipo / Clasificacion | Descripcion |
| | | |
| `index.html` | Archivo | Estructura HTML de la tienda con la llamada a estilos y scripts |
| `script.js` | Archivo | Logica en JS que realiza la suma y multiplicacion de productos |
| `git checkout -b` | Comando | Crea y cambia a una nueva rama de trabajo de forma simultanea |

---

## Bloque de Codigo de Ejemplo

Ejemplo de funcion corregida para procesar el importe total en el carrito:

```javascript
function calcularTotal(lista) {
  let total = 0;
  for (const producto of lista) {
    total = total + producto.precio * producto.cantidad;
  }
  return total;
}
```
