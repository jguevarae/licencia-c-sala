# Laboratorio de Tareas · Sesión 5 · cómo publicarlo y usarlo

## Qué trae este paquete

- `licencia-c-sala/`: el sitio completo. Lo nuevo es la carpeta `seleccion/` (la página de dinámicas de la Sesión 5) y la portada `index.html`, que ahora tiene la tarjeta del Laboratorio de Tareas. Las carpetas `medios/`, `esquemas/`, `clima/` y `metodos/` no cambiaron.
- `reglas-firebase.json`: las reglas de la base de datos. Traen una sección nueva, `seleccion`, para que el registro de la Sesión 5 funcione.
- `qr-seleccion.png`: el código QR de la página, por si lo quieres pegar en el chat o imprimirlo.

## 1. Subir el sitio a GitHub Pages

1. Entra a tu repositorio `licencia-c-sala` en GitHub, desde la computadora.
2. Toca **Add file → Upload files**.
3. Arrastra la carpeta `seleccion` y el archivo `index.html` que están dentro de `licencia-c-sala/` de este paquete. Si GitHub pregunta, reemplaza el `index.html` que ya existe.
4. Abajo, toca **Commit changes**.
5. Espera uno o dos minutos y abre https://jguevarae.github.io/licencia-c-sala/seleccion/ para comprobar que carga.

## 2. Poner las reglas de Firebase (una sola vez)

1. Abre la consola de Firebase, tu proyecto `licencia-c-sala`, y entra a **Realtime Database → Reglas**.
2. Borra lo que haya, pega el contenido completo de `reglas-firebase.json` de este paquete y toca **Publicar**.

Estas reglas traen las cuatro secciones: `clima`, `esquemas` (Sesión 3), `medios` (Sesión 4) y `seleccion` (Sesión 5). Si pegas las de una sesión anterior, la página de la Sesión 5 no podrá guardar. Igual que en las sesiones 3 y 4, nadie puede borrar ni cambiar lo que ya quedó registrado usando la página; para borrar una sala, hazlo desde la consola (pestaña **Datos**, `seleccion`, el nombre de la sala, la papelera).

## 3. Las dos direcciones

- **Para los entrenadores:** https://jguevarae.github.io/licencia-c-sala/seleccion/
- **Para ti, el instructor:** https://jguevarae.github.io/licencia-c-sala/seleccion/?instructor

Con `?instructor` aparecen el cronómetro, la pestaña **Registro**, una tarjeta en cada estación con cómo conducir la dinámica y la tarjeta **Lo que respondió la clase**. Tú no te registras y lo que toques no se guarda.

Para otro grupo usa otra sala, por ejemplo `?sala=grupo2` (y `?sala=grupo2&instructor` para ti).

## 4. Las seis dinámicas

| Hora | Estación | Dinámica | Tiempo |
|---|---|---|---|
| 6:00–6:27 | Inicio | El Duelo de la Pisada: tres escenas de 1 contra 1, encuesta y debate | 6 min |
| 6:27–7:00 | 1 · Criterios | ¿Sirve o hay que repararla?: seis tareas y la condición que les falta | 8 min |
| 7:00–7:30 | 2 · Progresión | Sube un escalón: el orden de la oposición y tres situaciones de la pared | 8 min |
| 7:45–8:15 | 3 · Picardía | Inventa la regla: tres reglas de provocación, picardía o trampa y su propia regla | 9 min |
| 8:15–8:48 | 4 · Portero | Rescata al portero: los errores del caso y el rediseño | 9 min |
| 8:48–9:15 | Cierre | Laboratorio de progresión: un gesto, tres tareas y el filtro | 15 min |

En cada estación, la tarjeta **Lo que respondió la clase** te da los números para la plenaria: qué eligieron, qué condición vieron, qué decidieron y las reglas que escribieron. En el cierre aparecen los laboratorios completos a medida que llegan, para escoger los de la plenaria.

## 5. Al terminar la clase

En la pestaña **Registro**:

1. **Descargar resumen por entrenador (CSV):** una fila por entrenador con sus resultados de las seis dinámicas y sus tres tareas del laboratorio.
2. **Cargar el registro completo** y después **Descargar registro completo (CSV):** cada acción de cada entrenador, con fecha y hora.
3. **Descargar todo (JSON):** una copia completa, para guardar.

## 6. Si algo falla

- **El entrenador ve «Registro sin permiso»:** faltan las reglas del paso 2. Lo que hizo queda en su teléfono y se envía en cuanto publiques las reglas.
- **Alguien no puede abrir la página:** al final de la estación **Cierre** está el botón **Copiar mi resumen**, para pegarlo en el chat.
- **Quieres probar antes de la clase sin mezclar datos:** usa `?sala=prueba` en las dos direcciones y, al terminar, borra la sala `prueba` desde la consola de Firebase.
